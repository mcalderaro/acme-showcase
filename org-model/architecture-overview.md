---
title: Architecture Overview
layout: page
section: org-model
permalink: /org-model/architecture-overview/
---

ACME ClawWorks is organized as an AI-assisted operating company rather than a single app.

At a high level, the model connects human direction, agent execution, tool access, and systems of record into one visible loop.

## The stack in plain language

The company operates through a layered structure:

- **Interfaces** where people give direction and review outcomes
- **Coordination services** that route work to the right agent or workflow
- **Agents** that carry defined roles and responsibilities
- **Tools** that let those agents inspect, write, search, and report
- **Systems of record** where tickets, code, and documentation live
- **Model providers** that supply reasoning and generation capability

That separation matters because it keeps ACME understandable. The public site is not just showing outputs. It is showing the structure that produced them.

## Core architectural idea

ACME is designed so that requests can start in natural language and still end up as traceable, reviewable work.

A human can describe a task conversationally. From there, the platform routes the work through systems that preserve intent, assign ownership, track progress, and capture results.

## Systems of record

Two systems anchor the operating model:

- **Plane** for tickets, status, backlog, and planning
- **GitHub** for repositories, branches, commits, pull requests, and public documentation

Agents operate on top of those systems. They do not replace them.

## Why the architecture exists

The point of the architecture is not maximum autonomy at any cost.

The point is to make AI-assisted work:

- observable
- reviewable
- role-aware
- easy to document
- easy to explain in public

That is what turns ACME from a demo into an organizational model.
