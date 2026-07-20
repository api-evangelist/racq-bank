---
name: Look up RACQ Bank banking products
description: >-
  Retrieve RACQ Bank's publicly offered banking products and their full detail
  via the unauthenticated CDR Product Reference Data API. No credentials
  required. Grounded in the DSB Consumer Data Standards Banking API.
api: openapi/racq-bank-cds-banking-products-openapi.yml
base_url: https://cdrbank.racq.com.au/cds-au/v1
operations:
  - listBankingProducts
  - getBankingProductDetail
---

# Look up RACQ Bank banking products

RACQ Bank exposes a **public, unauthenticated** Consumer Data Right (CDR)
Product Reference Data API. Use it to enumerate products and read their detail.
No API key, token, or accreditation is needed for these two operations.

## Prerequisites

- No authentication. Do **not** send an Authorization header.
- You **must** send a version header. Set `x-v: 5` (RACQ serves x-v 4 and 5).
  Omitting `x-v` returns `400`; requesting an unsupported version returns `406`.

## Steps

1. **List products** — call `listBankingProducts`:
   `GET https://cdrbank.racq.com.au/cds-au/v1/banking/products` with header `x-v: 5`.
   - Optional filters: `product-category`, `brand`, `effective`, `updated-since`.
   - Paginate with `page` and `page-size`. Read `meta.totalRecords` /
     `meta.totalPages` and follow `links.next` until absent.
   - Each item carries a `productId`.

2. **Get product detail** — for any `productId` from step 1, call
   `getBankingProductDetail`:
   `GET https://cdrbank.racq.com.au/cds-au/v1/banking/products/{productId}` with header `x-v: 5`.
   - Returns rates (`depositRates`, `lendingRates`), `fees`, `features`,
     `eligibility`, and `constraints` for that product.
   - A missing/invalid `productId` returns `404` with a CDS error envelope.

## Error handling

Errors use the CDS `ResponseErrorList` envelope, **not** RFC 9457:
`{ "errors": [ { "code": "urn:au-cds:error:v2:...", "title": "...", "detail": "..." } ] }`.
Handle `400` (bad field / missing x-v), `404` (unknown productId),
`406` (unsupported version). See `errors/racq-bank-problem-types.yml`.

## Notes

- This is read-only PRD data — no idempotency key needed.
- Account, balance, transaction, and payee operations in the same spec require
  the CDR accredited-data-recipient channel and are **not** usable here.
