# Tecnológico de Monterrey (tecnologico-de-monterrey)

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
