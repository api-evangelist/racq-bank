# RACQ Bank (racq-bank)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
