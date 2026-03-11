# Agent Examples

AgentLib currently ships three example agents in the `agent-examples` repository:

- `raul/code-reviewer`
- `acme/support-triager`
- `raul/docs-writer`

Each example is intentionally small, schema-valid, and portable.

## Shared structure

Each example currently includes:

- `agent.yaml`
- `agent.md`
- `README.md`
- `LICENSE`

This is the minimum practical package shape for the first iteration.

## Why these examples

The current set covers three distinct patterns:

- review and quality workflows
- operational triage workflows
- documentation generation workflows

That gives the registry a useful baseline without creating near-duplicate packages.

## Validation

From the `agent-examples` repo:

```bash
npm install
npm run validate
```

The validation script checks every example manifest against the canonical schema from `agent-schema`.
