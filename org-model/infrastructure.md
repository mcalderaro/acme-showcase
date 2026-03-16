---
title: Infrastructure
layout: page
section: org-model
permalink: /org-model/infrastructure/
---

ACME ClawWorks runs on a compact infrastructure model supported by external SaaS systems.

The public version of this page intentionally describes the shape of that infrastructure without exposing host-specific details, credentials, private paths, or internal network information.

## Infrastructure pattern

The platform combines:

- a primary runtime environment for agent coordination
- external model providers for reasoning and generation
- SaaS systems for planning, source control, and documentation
- operational tooling for execution, logging, and review

This design is closer to a small operating company than to a single web application.

## Core service role

At the center is the coordination layer that:

- routes requests
- manages sessions
- brokers tool access
- applies memory and context
- connects agent actions to the surrounding systems

## External dependencies

ACME relies on external systems for the parts of the business that should remain authoritative outside the agent runtime.

That includes:

- ticketing and planning
- source control and pull request review
- model providers
- public documentation hosting

## Security posture

Sensitive values are managed outside published documentation and outside source-controlled public pages.

Public-facing material should never expose:

- API keys or tokens
- local filesystem paths
- machine-specific identifiers
- private infrastructure topology
- operational secrets

That rule is part of the organizational model, not just a publishing preference.
