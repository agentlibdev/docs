# Publishing Example Agents

The current local registry flow supports manual publish with a JSON payload sent to `POST /api/v1/publish`.

## Recommended source examples

Use one of the examples from `agent-examples` as the source package:

- `examples/raul/code-reviewer`
- `examples/acme/support-triager`
- `examples/raul/docs-writer`

## Minimum publish inputs

The current alpha route expects:

- a valid manifest
- a README body
- a list of artifact metadata payloads

At minimum, package these files:

- `agent.yaml`
- `README.md`

## Local workflow

In the `agentlib` worktree:

```bash
npm run d1:reset:local
npm run dev:api:local
npm run publish:example:local -- ../agent-examples/.worktrees/examples-catalog/examples/raul/docs-writer
```

Then verify local persistence:

```bash
npm run d1:list:local
npm run d1:list:artifacts:local
```

The same flow works for:

- `../agent-examples/.worktrees/examples-catalog/examples/raul/code-reviewer`
- `../agent-examples/.worktrees/examples-catalog/examples/acme/support-triager`
- `../agent-examples/.worktrees/examples-catalog/examples/raul/docs-writer`

## Current limits

The current implementation:

- validates manifests against the AgentLib schema
- persists agent/version metadata in D1
- persists artifact metadata in D1
- does not upload artifact binaries to R2 yet
