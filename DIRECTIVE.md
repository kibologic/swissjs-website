# DIRECTIVE.md — SWISSJS WEBSITE / KIBOLOGIC AI OPERATING CONTRACT

**Version:** 1.0
**Mode:** Developer Documentation Site Specification
**Applies To:** All AI-assisted development in this repository

---

# 1. SYSTEM CONTEXT

## Project Identity

* **Project:** SwissJS Website
* **Type:** Developer-first framework site and documentation surface
* **Product Represented:** SwissJS, the framework and package ecosystem built in `kibologic/swiss-lib`
* **Audience:** Framework users, contributors, internal Kibologic developers, app teams evaluating SwissJS

---

## Stack

### Frontend

* SwissJS Framework
* `.ui` / `.uix` source files
* SwissJS component model
* Signal-based client-side routing

### Runtime / Tooling

* Swite dev server
* Node.js `dev.mjs` entry
* Local static asset serving via Express middleware

---

## Site Purpose

This repository is **NOT** a marketing site.

The site exists to help developers understand:

* what SwissJS is
* how the framework is structured
* what `.ui` and `.uix` are for
* how the runtime, compiler, router, plugins, and devtools fit together
* what packages exist in `swiss-lib`
* how to think in SwissJS when building applications

The site must be:

* technical
* documentation-oriented
* architecture-aware
* explicit about framework concepts
* grounded in the actual codebase

It must NOT become generic framework hype, vague comparison bait, or aesthetic-first filler.

---

## Product Truths

SwissJS must be represented accurately as:

* a framework monorepo, not a single package
* a runtime plus compiler ecosystem
* a system with custom `.ui` and `.uix` source formats
* a framework with component, context, routing, reactivity, security, plugins, and devtools surfaces
* a framework served and developed with Swite

If the site and `kibologic/swiss-lib` disagree, `swiss-lib` is the source of truth.

---

# 2. GIT OPERATING CONTRACT

## Branch Model

This repository has 3 required long-lived branches:

* `main` → production
* `staging` → pre-release validation
* `development` → active development base

If any are missing locally or remotely, they must be created before normal feature work continues.

---

## Feature Development Rule

All implementation work must follow:

```bash
development -> feature/<task-name> -> development -> staging -> main
```

---

## PR And Branch Cleanup Rule

Every feature branch must be:

* opened as a PR into `development`
* merged into `development` before the next task begins
* deleted remotely after merge
* deleted locally after merge

No stale feature branches should remain after a completed task.

---

## Required Workflow

### Step 1 — Before Work

AI must read:

* this full `DIRECTIVE.md`
* current repo status
* current branch
* relevant site files
* relevant SwissJS source files when product claims are involved

---

### Step 2 — During Work

* only change scoped website files
* do not edit framework repos from this repo
* do not invent framework concepts
* do not write generic marketing copy
* keep the site useful to developers first

---

### Step 3 — Completion Rule

Every completed task must:

* update this directive if project understanding changed
* update feature tracking state
* be committed
* be pushed to remote
* be opened as a PR into `development`
* be merged into `development`
* have the feature branch cleared locally and remotely

No task is complete without push, PR, merge, and branch cleanup.

---

# 3. AI EXECUTION LOOP

Every task must follow this loop:

## Step 1 — Load Context

Read:

* full `DIRECTIVE.md`
* relevant page/component files
* `package.json`
* `dev.mjs`
* real SwissJS source in `kibologic/swiss-lib` when needed

---

## Step 2 — Understand Scope

AI must identify:

* which framework concept is being represented
* which page(s) are affected
* which claims require repo verification

---

## Step 3 — Plan Minimally

Internal plan should cover:

* files to change
* framework source of truth
* user-facing outcome

No unnecessary redesign.

---

## Step 4 — Implement

Rules:

* reflect real framework behavior
* prefer clarity over ornament
* explain concepts in a way developers can use
* avoid generic AI site structure

---

## Step 5 — Verify

AI must ensure:

* site copy matches actual SwissJS behavior
* navigation still works
* layout remains readable for technical users
* examples and terminology align with the framework

---

## Step 6 — Finalize

Before task ends AI must:

* update feature tracking
* update this directive if needed
* commit changes
* push branch

---

# 4. FEATURE TRACKING SYSTEM

This is the live state for this site.

## Format

```md
## MODULE: Framework Positioning

- [x] Directive established
- [~] SwissJS concepts aligned with source
- [ ] package map documented clearly
```

---

## Current State

## MODULE: Repo Operations

- [x] `main` branch confirmed
- [x] `staging` branch created and pushed
- [x] `development` branch created and pushed
- [x] directive workflow adopted
- [x] current feature branch merged into `development`
- [x] merged feature branch cleared locally and remotely

## MODULE: Framework Accuracy

- [x] SwissJS positioning aligned with real codebase
- [x] boilerplate claims removed
- [x] package ecosystem explained correctly
- [x] unsupported claims removed

## MODULE: Information Architecture

- [x] landing page rewritten for developers
- [x] docs surface restructured
- [x] navigation aligned to real framework concepts
- [x] package map and ecosystem explained

## MODULE: Runtime Verification

- [x] site runs locally via `node dev.mjs`
- [x] key routes verified
- [x] content audited against `kibologic/swiss-lib`

---

# 5. CONTENT AND DESIGN GUARDRAILS

## Core Rules

* this is a framework site for developers
* concept clarity beats persuasion
* architecture beats aesthetics
* package structure matters
* examples and mental models matter more than slogans

---

## Design Rules

* design must feel deliberate and technical
* pages must be easy to scan
* framework concepts should be structurally visible
* avoid decorative sections with no instructional value

---

## Content Rules

* describe real SwissJS primitives and architecture only
* prioritize file model, runtime model, compiler model, package map, routing, reactivity, plugins, and devtools
* explain how SwissJS is used in Kibologic applications
* keep language crisp and technically credible

---

# 6. DIRECTIVE MAINTENANCE RULE

This file must be read before each task and updated after each meaningful task if:

* branch policy changes
* project purpose changes
* feature tracking changes
* new framework truths are discovered

If task state changes and this file is not updated, the repo memory is stale.

---

# 7. SESSION LOG

### 2026-04-18

* established repository directive
* created and pushed `development` and `staging`
* created `feature/directive-setup`
* locked workflow rule that every feature branch must PR into `development` and be cleared before the next task
* PR #1 merged into `development`
* `feature/directive-setup` cleared locally and remotely after merge
* rebuilt the SwissJS landing and docs surfaces around the real swiss-lib framework model
* removed generic framework promo copy and replaced it with runtime, compiler, package, file-model, and Swite integration content
* verified the rewritten site locally on temporary port `6101`

### 2026-04-24

* styling revamp started (developer-first, less generic)
* branch: `feature/swissjs-site-style-revamp`
