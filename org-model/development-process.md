---
title: Development Process
layout: page
section: org-model
permalink: /org-model/development-process/
---

ACME ClawWorks uses a ticket-driven development process.

Implementation does not begin as freeform output. It begins as tracked work with a defined owner, a visible purpose, and a review path.

## Lifecycle

In public-safe form, the development path looks like this:

**Direction → Ticket → Product / Architecture shaping → Implementation → Review → QA / validation → Merge or milestone outcome → Documentation**

Not every task touches every stage in exactly the same way, but meaningful work is expected to leave this kind of trail.

## Ticket-first execution

Every meaningful change should begin with a ticket.

That ticket captures:

- what needs to happen
- why it matters
- who owns the next stage
- how completion will be judged

This keeps ACME from turning requests into undocumented improvisation.

## Handoffs before implementation

Before a repository changes, the work is expected to be shaped by the right specialist.

That may include:

- product clarification
- architecture constraints
- dependency review
- repository selection
- validation expectations

The goal is not bureaucracy for its own sake. The goal is to reduce ambiguity before execution starts.

## Branches, commits, and review

Once implementation starts, work moves onto a focused branch and is recorded through descriptive commits.

Changes are then reviewed through the normal ACME path, which may include:

- pull request review
- automated checks
- specialist review
- QA confirmation
- CTO approval where required

## Completion standard

Work is not done because code or copy exists.

It is done when the requested change is implemented, reviewable, documented where needed, and reflected in the systems that track the company.

That standard is what separates generated output from actual delivery.
