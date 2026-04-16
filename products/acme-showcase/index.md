---
title: ACME Showcase
layout: page
permalink: /products/acme-showcase/
section: products
---

ACME Showcase is the public documentary site for ACME ClawWorks.

It is the product surface where ACME explains how the company works, publishes milestone and story content, and makes the operating model legible to outside readers.

## Purpose

This page is the product-local source-of-truth index for ACME Showcase.

It exists so future work does not have to reconstruct basic product facts from scattered tickets, branch names, or memory fragments.

## Canonical product docs

- [Technical Profile]({{ '/products/acme-showcase/technical-profile/' | relative_url }})
- [Architecture & Deployment Baseline]({{ '/products/acme-showcase/architecture-baseline/' | relative_url }})

## Current mapped product truth

- **Display name:** `ACME Showcase`
- **Plane project key:** `ACMESHOWCA`
- **Primary repository:** `mcalderaro/acme-showcase`
- **Repository role:** public-facing showcase site and documentary content source
- **Primary publishing target:** GitHub Pages for the `acme-showcase` site
- **Current site shape:** static content site with handbook-style navigation and product/story/milestone pages

## What lives where

- product-wide technical/runtime assumptions live in the [Technical Profile]({{ '/products/acme-showcase/technical-profile/' | relative_url }})
- deployment, publishing, and structural assumptions live in the [Architecture & Deployment Baseline]({{ '/products/acme-showcase/architecture-baseline/' | relative_url }})
- public narrative content lives in the main showcase sections, milestones, stories, and related pages

## Official vs provisional

The documents linked here describe the current official product baseline as reflected in the repository and active publishing setup.

If future tickets change Showcase architecture, hosting, or publication behavior, those changes should update these product-local docs so the repository remains the durable source of truth.
