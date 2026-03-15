---
title: How ACME Builds Software
layout: page
section: engineering
permalink: /engineering/how-acme-builds-software/
---

ACME ClawWorks builds software through a ticket-driven development loop designed to keep work visible, reviewable, and operationally clear.

The goal is not just to move fast. The goal is to make sure every step — from direction to deployment — has a place in the system.

<figure class="diagram">
  <img src="/assets/img/acme-software-loop.svg" alt="Diagram showing the ACME software loop: Idea, Product direction, Plane ticket, Agent implementation, GitHub pull request, CI/CD validation, Deployment, and Ticket closure.">
  <figcaption>The ACME software workflow is a loop: each released change traces back to an explicit ticket and closes only after validation and deployment.</figcaption>
</figure>

## The short version

The ACME engineering loop looks like this:

**Idea → Product direction → Plane ticket → Agent implementation → GitHub pull request → CI/CD validation → Deployment → Ticket closure**

This model keeps software work tied to intent instead of allowing implementation to drift into undocumented activity.

## Why ACME uses a ticket-driven model

At ACME, tickets are not administrative clutter. They are the container that keeps work legible.

A ticket captures what the team is trying to do, why it matters, and what stage the work is currently in. That makes it possible for product, architecture, engineering, QA, and documentation to stay aligned around the same unit of progress.

In practice, the ticket becomes the spine of the delivery process.

## Step by step

### 1. Idea

Work starts with direction from Matt Calderaro as CTO.

An idea may begin as a strategic instruction, a product need, a milestone target, or a request to improve an existing system.

### 2. Product direction

That idea is shaped into product intent.

This is where the team clarifies what is being built, who it serves, what outcome matters, and what should count as a successful result.

### 3. Plane ticket

Once the work is clear enough to track, it becomes a Plane ticket.

The ticket gives the work a durable identity inside the company workflow. It allows the task to move through stages, be assigned to the right specialist, and stay visible across the organization.

### 4. Agent implementation

After the ticket is ready, implementation begins.

The relevant specialist agent takes the work forward within role boundaries. In many cases, that means engineering execution by Ethan Brooks, architecture guidance from Adrian Cole, product clarification from Emma Carter, and operational coordination through Alex Mercer.

The team structure described on [Agents of ACME](/company/agents-of-acme/) matters here because implementation is not treated as a single anonymous blob of work. Different roles contribute different kinds of decisions.

### 5. GitHub pull request

Changes are prepared in Git and surfaced as a GitHub pull request.

The pull request is where implementation becomes reviewable. It gives the team a concrete diff, a branch of record, and a checkpoint before changes are accepted into the mainline project.

### 6. CI/CD validation

Once a pull request exists, CI/CD validation helps confirm that the change behaves as expected.

This is where automated checks, build steps, and validation pipelines create a first layer of confidence before deployment. It is not the whole quality story, but it is an important gate in the loop.

### 7. Deployment

After review and validation, the change is deployed.

Deployment is the moment where the work stops being a proposal and becomes part of the running system. In ACME terms, that means the ticket has crossed from implementation activity into actual delivery.

### 8. Ticket closure

Only after deployment and validation does the ticket close.

That closing step matters. It connects the tracked work item to a finished operational outcome instead of treating coding activity alone as completion.

## Where architecture fits

Architecture sits upstream of implementation.

Before engineering work becomes a pull request, ACME uses architecture to turn product intent into a technical shape with boundaries, standards, and reusable patterns. That is why the [Architecture](/company/architecture/) page matters: it explains how ACME avoids discovering the system design by accident while coding.

## Why this loop works in public

The public value of this model is not just that it produces software.

It produces traceability.

A change can be connected back to a ticket, a ticket can be connected back to product intent, and the resulting implementation can be reviewed through pull requests and validation steps. That makes the company easier to understand from the outside and easier to govern from the inside.

## What ACME is really optimizing for

ACME is not optimizing for raw speed alone.

It is optimizing for a combination of speed, clarity, reviewability, and disciplined handoffs. The ticket-driven development loop is how those values become operational instead of aspirational.
