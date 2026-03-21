---
title: Review and Publication Flow
layout: page
permalink: /operations/review-and-publication/
section: operations
---

ACME ClawWorks uses a review-first publication model.

That means public storytelling is treated as real work with source material, validation, branch history, and pull request review rather than as an informal final step after the fact.

## The public-safe flow

In plain language, the path looks like this:

**Direction → tracked ticket → implementation and validation → documentation draft → pull request review → approval → publication**

That sequence matters because it keeps the public site tied to actual company activity.

## Why review-first publication exists

The showcase is not meant to be a detached marketing layer.

It is supposed to describe real work that moved through the company. A review-first path helps ACME preserve that link by making publication depend on artifacts that can be checked:

- tickets
- milestone records
- implementation outputs
- validation results
- draft pages and pull requests

## Nora’s role in the flow

Nora Hale owns the documentation and showcase side of the handoff.

That includes:

- auditing whether the public story matches current company reality
- drafting milestone pages, stories, and company explainers
- preparing changes on a focused branch
- opening a pull request for Matt’s review
- waiting for approval before anything is treated as published

This keeps public storytelling aligned with the same review discipline used elsewhere in ACME.

## What gets checked before publication

Before a public change is ready for review, ACME expects basic validation such as:

- the story is accurate to the current operating model
- role ownership and approvals are described correctly
- no private links, secrets, or internal-only details are exposed
- the draft is organized in a way that future updates can maintain cleanly

The goal is not to slow everything down. The goal is to keep the public record dependable.

## What publication means at ACME

Publication is not the moment a draft exists.

Publication happens after review, approval, merge, and deployment through the normal site path. That distinction sounds small, but it is one of the clearest signs that ACME treats public documentation as a governed outcome instead of a casual side effect.
