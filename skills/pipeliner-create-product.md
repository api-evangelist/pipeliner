---
name: pipeliner-create-product
description: Create a new Product and retrieve its details.
api: openapi/pipeliner-openapi.json
operations:
- Products.create
- Products.get
generated: '2026-09-22'
method: generated
generator: extract-docs-artifacts.py skills (local)
source: openapi/pipeliner-openapi.json ; every operationId checked against the contract
---

# pipeliner-create-product

Create a new Product and retrieve its details.

## Steps

1. 1. Call `Products.create` with the required product fields in the request body.
2. 2. Call `Products.get` using the `id` returned from the create operation.

## Rules

- Include the authentication header as required by the API.
- The `Products.create` operation is not idempotent; avoid duplicate requests.
- When listing products, use pagination parameters `first` (default 30, max 100) and `after`.
