---
title: ACME Showcase Architecture & Deployment Baseline
layout: page
permalink: /products/acme-showcase/architecture-baseline/
section: products
---

# ACME Showcase — Architecture & Deployment Baseline

## Purpose

This page is the current official architecture and deployment baseline for ACME Showcase.

It exists so future work can answer questions like _where is Showcase deployed?_ and _what is the source of truth for site structure?_ without reconstructing prior ticket history.

## Product role

ACME Showcase is the public-facing documentary layer for ACME ClawWorks.

Its architecture is intentionally simple: a repository-backed static site that turns authored Markdown content and shared layout/templates into a published public website.

## Current architecture shape

### Authoring layer
Authors work in the Git repository by updating:

- Markdown pages
- Jekyll collections
- layout and include templates
- navigation data
- CSS and image assets

### Build layer
The repository contains GitHub Actions workflows that:

- run content checks on pull requests
- build the Jekyll site
- prepare the site artifact for publication

### Hosting layer
The built site is currently published through **GitHub Pages**.

That means the public runtime is a generated static site rather than a long-running application process managed by ACME infrastructure.

## Current deployment baseline

### Source repository
- **Repository:** `mcalderaro/acme-showcase`
- **Default delivery branch:** `main`

### Build and deploy path
Current expected publication flow:

1. changes are developed in a branch
2. changes are reviewed through a pull request
3. pull request validation runs the content-check workflow
4. merges or direct pushes to `main` trigger the Pages workflow
5. GitHub Pages publishes the generated site

### Site configuration baseline
Current repository evidence shows:

- site configuration lives in `_config.yml`
- the current configured base URL is `/acme-showcase`
- permalink style is `pretty`
- milestones, devlogs, stories, team profiles, and products are configured as output collections

## Structural source of truth

The current structural source of truth is split deliberately across a few repository-local files:

- `_config.yml` — site-wide output and URL behavior
- `_data/handbook_nav.yml` — primary navigation structure
- content directories and collection entries — public information architecture
- layouts/includes/assets — presentation layer shared across pages

For future work, the rule should be simple:

- if the question is about site routing or content output behavior, start with `_config.yml`
- if the question is about visible handbook navigation, start with `_data/handbook_nav.yml`
- if the question is about product-specific Showcase truth, start with the product pages under `/products/acme-showcase/`

## Environment model

### Current practical environments
At the current baseline, Showcase effectively has two practical environments:

1. **Local authoring/review environment**
   - repository checkout used for editing and validation
   - branch-based work before merge

2. **Published GitHub Pages environment**
   - static generated public site
   - updated from the repository's delivery workflow

There is no evidence in the repository that Showcase currently depends on a separate app server, database environment, or private runtime host for normal public delivery.

## Explicit current non-goals

The current Showcase baseline does not require:

- backend services
- application databases
- authenticated runtime state
- product-specific server infrastructure for the public site
- bespoke deployment hosts outside the GitHub publication path

## Official vs provisional

### Official now
The following should be treated as official current baseline:

- Showcase is repository-authored
- Showcase is statically built
- Showcase deploys through GitHub Actions to GitHub Pages
- navigation and page structure are repository-local and version controlled

### Provisional / subject to future tickets
The following may change later and should be updated here if they do:

- the hosting platform
- the site generator
- the exact publication workflow details
- whether Showcase gains richer dynamic behavior beyond the current static model

## Operational guidance for future tickets

When future tickets change public Showcase structure or content:

- update the repository content and navigation together
- preserve a coherent public URL structure
- keep product-local source-of-truth docs current when stack or deployment assumptions change
- avoid forcing future agents to infer architecture from scattered implementation clues
