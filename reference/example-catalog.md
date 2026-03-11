# Example Catalog

## `raul/code-reviewer`

Purpose:
Review pull requests and return concise technical findings.

Primary inputs:
- `repository`
- `diff`
- `context`

Primary outputs:
- `summary`
- `findings`

## `acme/support-triager`

Purpose:
Classify inbound support requests and recommend queue plus urgency.

Primary inputs:
- `ticket`
- `history`

Primary outputs:
- `severity`
- `route`
- `summary`

## `raul/docs-writer`

Purpose:
Draft developer documentation and change summaries from source material.

Primary inputs:
- `source`
- `audience`

Primary outputs:
- `draft`
- `changelog`
