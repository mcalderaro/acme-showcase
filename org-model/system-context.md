---
title: System Context
layout: page
section: org-model
permalink: /org-model/system-context/
---

The ACME system context describes the environment around the platform: who interacts with it, which systems it depends on, and where authority lives.

## Primary participants

The model includes three broad participant groups:

- **Human operators** who direct work, review outcomes, and set priorities
- **Agents** who carry out defined responsibilities inside the operating model
- **External users or viewers** who interact with public or messaging-facing surfaces

## External systems

Several outside systems play important roles in the ACME model:

- a ticketing platform for planning and work state
- GitHub for code and repository history
- model providers for reasoning and generation
- public documentation surfaces for publication and review

## Interfaces

People and agents interact through a mix of conversational interfaces, web surfaces, and command-line workflows.

That multi-interface design is deliberate. ACME is meant to support both natural-language direction and structured operational work.

## Architectural principle

The key idea is simple:

**agents operate the systems of record; they do not replace them.**

That keeps authority clear and makes the company easier to audit, explain, and document.
