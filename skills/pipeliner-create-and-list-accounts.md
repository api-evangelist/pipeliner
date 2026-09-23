---
name: pipeliner-create-and-list-accounts
description: Create a new Account and then retrieve a list of Accounts.
api: openapi/pipeliner-openapi.json
operations:
- Accounts.create
- Accounts.list
generated: '2026-09-22'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/pipeliner-openapi.json ; every operationId checked against the contract
---

# pipeliner-create-and-list-accounts

Create a new Account and then retrieve a list of Accounts.

## Steps

1. 1. Use `Accounts.create` with the request body fields required for an Account.
2. 2. Use `Accounts.list` with optional query parameters `first` (default 30, max 100) and `after` for pagination.

## Rules

- Pagination: use the `first` query parameter (default 30, max 100) and the `after` cursor for paging through results.
