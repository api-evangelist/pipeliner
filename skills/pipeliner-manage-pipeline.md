---
name: pipeliner-manage-pipeline
description: Create a new pipeline, retrieve it, update its details, and list pipelines with pagination.
api: openapi/pipeliner-openapi.json
operations:
- Pipelines.create
- Pipelines.get
- Pipelines.update
- Pipelines.list
generated: '2026-09-22'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/pipeliner-openapi.json ; every operationId checked against the contract
---

# pipeliner-manage-pipeline

Create a new pipeline, retrieve it, update its details, and list pipelines with pagination.

## Steps

1. 1. Call `Pipelines.create` with the required request body fields for a new pipeline.
2. 2. Call `Pipelines.get` with the `id` path parameter returned from the create step.
3. 3. Call `Pipelines.update` with the `id` path parameter and the fields to modify in the request body.
4. 4. Call `Pipelines.list` using the pagination parameters `first` (default 30, max 100) and optional `after` cursor.

## Rules

- Pagination uses the `first` query parameter (default 30, maximum 100) and the `after` cursor for subsequent pages.
