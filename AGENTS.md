# AGENTS.md

This file defines repo-specific operating rules for `docs`.

The root [AGENTS.md](/home/raul/agentlibdev/AGENTS.md) still applies. This file narrows execution for the documentation repository.

## Mission

Document AgentLib so contributors and users can understand:

- the specification
- the registry architecture
- the publishing flow
- contributor workflows
- the future CLI surface

## Scope

This repo owns:

- getting started guides
- publishing guides
- schema guides
- architecture notes
- API documentation
- contributor documentation

This repo does not own:

- canonical schema definitions
- executable registry code
- example agent packages

## Documentation Principles

Prefer:

- short pages with clear ownership
- concrete examples over abstract language
- exact commands when possible
- direct links to the owning repo for canonical details

Avoid duplicating source-of-truth content that belongs in other repos. Summarize and link instead.

## Initial Structure

Prefer:

- `guides/`
- `architecture/`
- `reference/`
- `plans/`

Suggested first pages:

- getting started
- schema guide
- publishing guide
- registry architecture overview
- API reference

## Sync Rules

Docs must move with behavior.

When a contract changes in another repo:

- update the relevant guide or reference here in the same work cycle
- link to the canonical source
- note any migration or compatibility implication

## Writing Rules

Write for fast comprehension:

- define terms once
- avoid marketing language
- prefer examples, tables, and short sections
- keep speculative roadmap material clearly separated from current behavior

## Approval Gates For This Repo

Ask before:

- publishing guidance that freezes public naming conventions
- documenting a workflow as official before implementation exists
- introducing major architecture narratives that commit other repos to a direction

## Execution Priority

Unless directed otherwise, use this order:

1. architecture overview
2. schema guide
3. getting started
4. publishing guide
5. API reference

## Definition of Done

Work in this repo is done when:

- docs match the implemented behavior
- canonical sources are linked
- contributor-facing steps are reproducible

