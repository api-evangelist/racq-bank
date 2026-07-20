# RACQ Bank (racq-bank)

RACQ Bank is the retail banking division of RACQ (The Royal Automobile Club of Queensland), a member-owned mutual organisation and one of Queensland's largest clubs, long known for roadside assistance, insurance, and banking for its members. The bank is an Australian authorised deposit-taking institution (ADI) regulated by APRA, offering transaction and savings accounts, term deposits, home loans, personal loans, and credit cards. Its banking arm traces to QT Mutual Bank, which merged with RACQ in 2016. As an active data holder under Australia's Consumer Data Right (CDR / Open Banking), RACQ Bank exposes a public, unauthenticated Product Reference Data (PRD) API conforming to the DSB Consumer Data Standards.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/racq-bank/refs/heads/main/apis.yml)

## Tags

- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Australia
- Product Reference Data
- ADI
- Mutual

## Timestamps

- **Created:** 2026-07-20
- **Modified:** 2026-07-20

## APIs

### RACQ Bank CDR Product Reference Data API

Public, unauthenticated Consumer Data Right Product Reference Data (PRD) API exposing RACQ Bank's publicly available banking products (transaction and savings accounts, term deposits, home and personal loans, credit cards) via the standard CDS endpoints `GET /banking/products` and `GET /banking/products/{productId}`. Confirmed live (HTTP 200, `x-v: 4` and `x-v: 5`, 39 products) at the base URL below.

- **Human URL:** [https://www.racq.com.au/banking/open-banking/api-access](https://www.racq.com.au/banking/open-banking/api-access)
- **Base URL:** `https://cdrbank.racq.com.au/cds-au/v1`

#### Tags

- CDR
- Open Banking
- Product Reference Data
- Banking
- Australia

#### Properties

- [Documentation](https://www.racq.com.au/banking/open-banking/api-access)
- [API Reference](https://consumerdatastandardsaustralia.github.io/standards/#banking-apis)
- [OpenAPI](openapi/racq-bank-cds-banking-products-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Common Properties

- [Website](https://www.racq.com.au/)
- [Documentation](https://www.racq.com.au/banking/open-banking/api-access)
- [Portal](https://www.racq.com.au/banking/open-banking)
- [LinkedIn](https://www.linkedin.com/company/racq/)
- [Support](https://www.racq.com.au/banking/support-and-faqs)
- [Privacy Policy](https://www.racq.com.au/privacy-policy)
- [Terms of Service](https://www.racq.com.au/legal)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
