---
title: ACME Showcase Technical Profile
layout: page
permalink: /products/acme-showcase/technical-profile/
section: products
---

# ACME Showcase — Technical Profile

## Status

Current documented baseline.

This page captures the current technical reality of ACME Showcase based on the live repository and active publication workflow.

## Product type

ACME Showcase is a **static public website**.

Its primary job is to publish durable explanatory content about ACME ClawWorks rather than provide an authenticated application runtime.

## Core stack

### Site generator
- **Jekyll**
- **Markdown** content
- **Liquid** templating/front matter conventions used by Jekyll

### Hosting / publication platform
- **GitHub Pages**
- **GitHub Actions** for build and deployment workflow execution

### Frontend shape
- static HTML pages generated from Markdown and layout templates
- shared includes for navigation and footer structure
- site CSS in `assets/css/site.css`
- image assets under `assets/img/`

### Content model
Current content is organized through a mix of pages and Jekyll collections, including:

- company pages
- organizational model pages
- engineering pages
- operations pages
- milestones
- stories
- team profiles

## Repository and content structure

The repository serves as both:

1. the source of the public documentary content
2. the source of the site structure and build configuration

Important current files and directories include:

- `README.md` — repository-level introduction
- `_config.yml` — Jekyll site configuration and collection output rules
- `_data/handbook_nav.yml` — handbook-style navigation structure
- `_layouts/` — shared page/layout templates
- `_includes/` — reusable site fragments
- `assets/` — CSS and image assets
- top-level content folders such as `company/`, `engineering/`, `operations/`, `org-model/`, and `products/`

## Publishing model

The current publishing model is:

- content and structural changes are committed in Git
- pull requests are used for reviewable changes
- GitHub Actions validates content on pull requests
- pushes to `main` trigger the Pages deployment workflow
- the built site is published through GitHub Pages

## What Showcase is not

At the current baseline, Showcase is not:

- a server-rendered application with a persistent backend runtime
- a login-protected product surface
- a database-backed content management system
- a multi-service or infrastructure-heavy application stack

## Official assumptions

The following should be treated as current official product truth unless a later ticket changes them:

- Showcase is a static site product
- Jekyll is the site-generation layer
- GitHub Actions + GitHub Pages are the current publication path
- repository-managed Markdown content is the primary authoring model

## Still provisional

These points should be treated as current reality, but still subject to future ticketed change:

- how far product-local docs should expand beyond the current baseline set
- whether Showcase eventually adds richer content-generation or automation tooling
- whether the site stays on the current Jekyll/GitHub Pages stack long term
