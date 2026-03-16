---
title: Repository Structure
layout: page
section: org-model
permalink: /org-model/repository-structure/
---

ACME ClawWorks uses a repository structure that follows product and system boundaries.

The goal is not to create dozens of repositories for their own sake. The goal is to keep ownership, change history, and documentation easy to reason about.

## Organizing principle

A repository should represent a meaningful product or system boundary.

That means code, configuration, and documentation tend to live close to the work they support, instead of being scattered across unrelated locations.

## What repositories typically contain

Depending on the product, a repository may include:

- application code
- documentation
- configuration
- scripts and automation
- tests

Not every repository needs the same shape. The structure should fit the system it represents.

## Branching and review

ACME uses branch-based development so changes can be isolated, reviewed, and merged cleanly.

The important part is not the exact branch prefix. It is that work stays scoped, traceable, and tied back to the ticket that requested it.

## Documentation inside repositories

Repositories are expected to carry the documentation needed to understand and maintain the system.

That may include:

- README files
- architecture notes
- workflow references
- operational guidance

## Security rule

Repositories must never become a dumping ground for secrets or environment-specific details.

The public side of ACME can explain how the company is organized without exposing values or internals that do not belong in source control.
