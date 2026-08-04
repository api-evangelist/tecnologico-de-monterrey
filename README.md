# Tecnológico de Monterrey (tecnologico-de-monterrey)

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

Tecnológico de Monterrey (ITESM) is a private Mexican multi-campus university system headquartered in Monterrey, ranked #185 in the QS World University Rankings 2025. This repository catalogs its public developer and API footprint as an [APIs.json](https://apisjson.org) provider profile for the API Evangelist network.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/tecnologico-de-monterrey/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=tecnologico-de-monterrey-api-evangelist&utm_content=repo

## Type

- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

Education, Higher Education, University, Open Data, Research Data, Mexico, Dataverse, OAI-PMH

## APIs

- **Tec de Monterrey Dataverse Native REST API** — Public Native REST API of the research open-data repository (Dataverse 5.9). Docs: https://guides.dataverse.org/en/5.9/api/native-api.html — Base: https://datahub.tec.mx/api
- **Tec de Monterrey Dataverse OAI-PMH Endpoint** — Public OAI-PMH 2.0 metadata harvesting endpoint ("Tecnológico de Monterrey Dataverse OAI Archive"). Docs: https://guides.dataverse.org/en/5.9/api/oai.html — Base: https://datahub.tec.mx/oai
- **RITEC Institutional Repository OAI-PMH (DSpace)** — DSpace repository (80,000+ works) with a documented OAI-PMH endpoint; registry-listed but blocks programmatic clients. Docs: https://v2.sherpa.ac.uk/id/repository/3460 — Base: https://repositorio.tec.mx/oai/request
- **Tec de Monterrey API Developer Portal (Institutional APIs)** — Gated portal of institutional API products (student grades, academic progress, student management, human-capital management, billing). Docs: https://api.tec.mx/tec-de-monterrey/api/

## Plans / Rate Limits / FinOps

- [Plans & Pricing](plans/tecnologico-de-monterrey-plans-pricing.yml)
- [Rate Limits](rate-limits/tecnologico-de-monterrey-rate-limits.yml)
- [FinOps](finops/tecnologico-de-monterrey-finops.yml)

## Timestamps

- **Created:** 2026-06-03
- **Modified:** 2026-06-03

## Common Properties

- Website: https://tec.mx/en
- GitHub: https://github.com/tecnologico-de-monterrey-oficial
- LinkedIn: https://www.linkedin.com/school/tecdemonterrey/
- Developer Portal: https://api.tec.mx/tec-de-monterrey/api/

## Notes

- The **datahub.tec.mx** research data hub was independently verified live: Dataverse `/api/info/version` returned version 5.9, `/api/search` returned HTTP 200, and the OAI-PMH `Identify` verb returned a valid response.
- The **api.tec.mx** developer portal is genuine and hosts multiple named API products, but is gated behind account registration and per-product subscription approval. It refused automated/programmatic fetches (returns to a browser only), so its individual endpoints could not be independently verified. No endpoints were fabricated.
- See [review.yml](review.yml) for per-URL verification status.

## Maintainers

- Kin Lane — kin@apievangelist.com
