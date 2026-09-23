---
name: pipeliner-client-list-and-fetch
description: Retrieve a paginated list of clients and fetch full details for each client.
api: openapi/pipeliner-openapi.json
operations:
- Clients.list
- Clients.get
generated: '2026-09-22'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/pipeliner-openapi.json ; every operationId checked against the contract
---

# pipeliner-client-list-and-fetch

Retrieve a paginated list of clients and fetch full details for each client.

## Steps

1. 1. Call `Clients.list` with pagination parameters `first` (default 30, max 100) and `after` to obtain a page of client IDs.
2. 2. For each client ID returned, call `Clients.get` supplying the path parameter `id` to retrieve the client’s full record.

## Rules

- Pagination: use the `first` query parameter (default 30, maximum 100) and the `after` cursor for subsequent pages.
