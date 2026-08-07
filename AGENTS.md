# AGENTS Instructions

Project guidance for coding agents working on taranis.ai.

## Agent Persona

Name: jipitiii

## Project Overview

taranis.ai is an OSINT application. See [README.md](README.md) for product context.

## Required Reading

- Before editing application code or running validation, read [Development Workflow](docs/agents/development-workflow.md).
- Before editing `src/core`, `src/frontend`, `src/worker`, models, API boundaries, queues, persistence, or datetime handling, also read [Architecture and Boundaries](docs/agents/architecture-and-boundaries.md).
- For an application feature, workflow, route, model, template, or user-facing behavior, first inspect [Agent Memory](docs/agents/README.md) and read every matching memory before planning or editing.

Memory files provide expected behavior, code paths, tests, and known pitfalls; implementation remains the source of truth. Update a matching memory when behavior, code paths, cache behavior, validation, or test strategy changes. Add and index a memory for substantial recurring workflows.

## Public Documentation

Public user, administrator, operator, deployment, and API documentation lives in the sibling `../taranis.ai` (`not4Pedro/taranis.ai`) repository. Changes to user-visible behavior, configuration, defaults, permissions, APIs, deployment, upgrades, collectors, bots, connectors, presenters, or publishers may require a documentation update; mark the pull request with the `documentation` label when it does.

Use this repository's implementation and tests as the source of truth. Files under `docs/agents/` are internal engineering memory: use them to find relevant behavior and pitfalls, but do not copy them directly into public documentation.
