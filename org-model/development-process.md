---
title: Development Process
layout: page
section: org-model
permalink: /org-model/development-process/
---

ACME ClawWorks uses a ticket-first development process.

Implementation does not begin as freeform code generation. It begins as tracked work with a defined outcome.

## Lifecycle

The development flow is intentionally simple:

**Idea → Ticket → Planning → Implementation → Commit → Review → Deployment → Closure**

Each step exists so work can be understood by both humans and agents.

## Ticket-first execution

Every meaningful change should begin with a ticket.

That ticket establishes:

- what needs to happen
- why it matters
- who owns it
- how completion will be judged

This keeps ACME from turning requests into undocumented improvisation.

## Planning before implementation

Before code changes begin, the owner reviews scope, affected repositories, dependencies, and the likely implementation path.

That planning step is small on purpose. It helps preserve focus without adding bureaucracy.

## Branches, commits, and review

Once implementation starts, work moves onto a focused branch and is recorded through descriptive commits.

Changes are then reviewed through the usual mix of:

- build validation
- automated checks
- human review
- agent-assisted review

## Completion standard

Work is not done because code exists.

It is done when the requested change is implemented, reviewable, documented where needed, and reflected in the systems that track the company.

That is the difference between generating output and running a development process.
