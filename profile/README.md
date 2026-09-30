# Blueprint4Agent

Blueprint4Agent is an **organization for agentic coding web server blueprints (templates)**.
It is designed with a **de facto first** approach for practical adoption and optimized for agentic automation workflows.

At the moment, the organization provides a **FastAPI-based full-stack blueprint** whose frontend is the shared **B4React** repository, pinned as a Git submodule.
A **Spring Boot** blueprint (**B4SpringBoot**) is being added next, reusing the same B4React frontend and API contract.
Additional web server framework blueprints such as **Node.js** will follow in later phases.

The ultimate goal is to let teams adopt this organization structure as-is and run GitHub projects in an **agentic coding workflow** from day one.

## Goals

- Provide a documentation website via GitHub Pages + Docusaurus
- Provide baseline templates for specs, manuals, and project documentation
- Provide a shared frontend (B4React) that multiple backend blueprints consume through a common API contract
- Provide automation flows for project review and issue creation via agent automation bots

## Repository Structure

```text
Blueprint4Agent/
├── AGENTS.md
│   └── English top-level local agent guide for managing the multi-repository B4A workspace
├── AGENTS.ko.md
│   └── Korean top-level local agent guide for managing the multi-repository B4A workspace
├── .github
│   ├── AGENTS.md
│   ├── AGENTS.ko.md
│   └── Organization profile, shared policies, workflow templates
├── Blueprint4Agent.github.io
│   └── Docusaurus-based project documentation website (GitHub Pages)
├── B4FastAPI
│   └── FastAPI-based full-stack web server blueprint (B4React frontend as a submodule)
├── B4React
│   └── Shared React + TypeScript frontend for B4 API backends (optional Tauri desktop shell)
├── B4SpringBoot
│   └── Spring Boot-based web server blueprint (planned)
└── B4Bot
    └── Agent-based project management bot and scoped issue-generation action
```

When composing a local B4A workspace, place `AGENTS.md` and `AGENTS.ko.md` at the top-level root above the individual repositories.
Use them as the root coordination guides for the multi-repository structure, repository boundaries, required read order, and agent workflow rules.

The `.github` repository includes `AGENTS.md` and `AGENTS.ko.md` at its repository root as the source references for this setup.
Configure those guides in the actual local workspace root, not only inside an individual repository checkout.

## Direction

Blueprint4Agent is not only about code templates.
It aims to provide an **agentic development foundation** across code, documentation, automation, and review workflows.

---

For Korean, see [README.ko.md](./README.ko.md).
