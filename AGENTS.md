# Agent Guide

This repository is the `.github` repository for the GitHub organization `Blueprint4Agent`.

Korean version: `AGENTS.ko.md`

## Repository Scope

This repository manages organization-level GitHub presentation and shared organization metadata.

Primary contents:

- `profile/README.md`: English organization profile README
- `profile/README.ko.md`: Korean organization profile README
- `AGENTS.md`: source guide for configuring the top-level local B4A workspace agent guide
- `AGENTS.ko.md`: Korean source guide for configuring the top-level local B4A workspace agent guide

## Local B4A Workspace Setup

When composing a local Blueprint4Agent workspace, create or place `AGENTS.md` and `AGENTS.ko.md` at the top-level root above the individual repositories.

Recommended local layout:

```text
blueprint4agent/
├── AGENTS.md
├── AGENTS.ko.md
├── .github/
├── B4FastAPI/
├── B4React/
├── B4SpringBoot/  # planned
├── B4Bot/
└── Blueprint4Agent.github.io/
```

Use this repository's `AGENTS.md` and `AGENTS.ko.md` as the source reference for those top-level local guide files.
The top-level local guide must describe the multi-repository structure, repository boundaries, required read order, and agent workflow rules.

## Repository Boundaries

- Keep organization-wide profile content in `profile/`.
- Keep implementation details in the repository that owns the implementation.
- Do not place B4FastAPI-, B4React-, B4SpringBoot-, B4Bot-, or Docusaurus-specific technical details in this repository unless they are part of the organization overview.
- Keep English and Korean profile README content synchronized.
- Maintain `AGENTS.md` and `AGENTS.ko.md` together.

## Required Read Order

When working in this repository:

1. `AGENTS.md` or `AGENTS.ko.md`
2. `profile/README.md`
3. `profile/README.ko.md`

When working in a full local B4A workspace:

1. Top-level workspace `AGENTS.md` or `AGENTS.ko.md`
2. Target repository `AGENTS.md` or `AGENTS.ko.md`, if present
3. Target repository domain guides and README files

## Documentation Policy

- Default language for organization-level documentation is English.
- Korean documentation is maintained in parallel when present.
- If the organization structure changes, update both `profile/README.md` and `profile/README.ko.md`.
- If local workspace setup guidance changes, update this file, `AGENTS.ko.md`, and the profile README files in the same work cycle.

## Verification

This repository mainly contains Markdown.

- Check Markdown readability after edits.
- Run `git status --short` from this repository before committing.
- Confirm only intended profile or guide files are changed.
