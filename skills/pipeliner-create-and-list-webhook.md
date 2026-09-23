---
name: pipeliner-create-and-list-webhook
description: Create a new webhook and then retrieve it from the list of webhooks.
api: openapi/pipeliner-openapi.json
operations:
- Webhooks.create
- Webhooks.list
- Webhooks.get
generated: '2026-09-22'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/pipeliner-openapi.json ; every operationId checked against the contract
---

# pipeliner-create-and-list-webhook

Create a new webhook and then retrieve it from the list of webhooks.

## Steps

1. 1. Use `Webhooks.create` with the request body fields required to define the webhook.
2. 2. Use `Webhooks.list` with optional pagination parameters `first` (default 30, max 100) and `after` to locate the newly created webhook.
3. 3. Use `Webhooks.get` with the `id` path parameter of the webhook returned from the list to retrieve its full details.

## Rules

- Pagination: `Webhooks.list` supports `first` (default 30, max 100) and `after` query parameters.
- Idempotency: Not specified in the documentation; callers should ensure unique webhook definitions when creating.
