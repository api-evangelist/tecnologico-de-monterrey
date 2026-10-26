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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
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

University, Higher Education, Education, Mexico, Private Research University, Research Data, Open Data, Research Repository, Institutional Repository, Identity Federation, OAI-PMH, Dataverse, DSpace, SAML, Shibboleth, DataCite, Crossref

## Surfaces

Every entry carries an `x-operator` in `apis.yml`: `institution` (they run it), `federation`
(shared identity federation carrying their own IdP) or `registry` (an identifier registry they are
registered in). **No OpenAPI is saved under this institution** — see Notes.

- **Datahub Tec de Monterrey — Dataverse Research Data Repository API** (`institution`) — Public, keyless read API of the research open-data repository, Dataverse 5.9. Base: https://datahub.tec.mx/api
- **Datahub Tec de Monterrey — OAI-PMH Metadata Harvesting Endpoint** (`institution`) — Identify verified 2026-09-01. Base: https://datahub.tec.mx/oai
- **RITEC Institutional Repository — DSpace REST API** (`institution`) — DSpace 8.0, 86,310 objects, public HAL+JSON. Base: https://repositorio.tec.mx/server/api
- **RITEC Institutional Repository — OAI-PMH Endpoint** (`institution`) — Identify verified 2026-09-01. Base: https://repositorio.tec.mx/server/oai/request
- **Tec de Monterrey AD FS Identity Provider (fs.itesm.mx)** (`institution`) — SAML 2.0 metadata + OIDC discovery, on the institution's own domain.
- **Tec de Monterrey Access Manager Identity Provider (amfs.tec.mx)** (`institution`) — NetIQ Access Manager SAML 2.0 IdP metadata.
- **RITEC Shibboleth Service Provider** (`institution`) — SP metadata at /Shibboleth.sso/Metadata, advertised in the DSpace REST `WWW-Authenticate` header.
- **Microsoft Entra ID Tenant Federation Metadata** (`federation`) — tenant c65a3ea6-0f7c-400b-8934-5a6dc1705645 covering tec.mx and itesm.mx.
- **DataCite Membership — ITESM** (`registry`) — consortium organization, prefix 10.57687, three repositories.
- **Crossref Membership — member 25649** (`registry`) — prefix 10.46530, 430 DOIs.
- **ROR Registration — 03ayjn504** (`registry`).

## Conformance

- [Domain standard conformance](conformance/tecnologico-de-monterrey-conformance.yml) — `education` regime. Conformant with evidence: **oai-pmh, saml, shibboleth, datacite, crossref**. Probed and absent: orcid, scim, lti, oneroster, ed-fi, caliper, qti.

## Plans / Rate Limits / FinOps

- [Plans & Pricing](plans/tecnologico-de-monterrey-plans-pricing.yml)
- [Rate Limits](rate-limits/tecnologico-de-monterrey-rate-limits.yml)
- [FinOps](finops/tecnologico-de-monterrey-finops.yml)

## Timestamps

- **Created:** 2026-06-03
- **Modified:** 2026-09-01

## Common Properties

- Website: https://tec.mx/en
- Open Data: https://datahub.tec.mx/
- Research Repository: https://repositorio.tec.mx/
- Identity Federation: https://fs.itesm.mx/FederationMetadata/2007-06/FederationMetadata.xml
- AI Policy: https://tec.mx/en/academic-integrity/artificial-intelligence
- GitHub: https://github.com/tecnologico-de-monterrey-oficial
- LinkedIn: https://www.linkedin.com/school/tecdemonterrey/

## Notes

- **No OpenAPI is attributed to this institution, deliberately.** The 22 OpenAPI documents this
  repository previously held were 22 per-tag splits of a single document served at
  https://datahub.tec.mx/openapi. That document is generated at runtime by the Dataverse / Payara
  MicroProfile stack: its live `info.title` is `Deployed Resources` and its `servers` are internal
  deployment hosts. It is the Dataverse project's contract, identical across every Dataverse
  install — the deployment is the institution's, the contract is not. The same reasoning applies to
  the DSpace REST API. Both surfaces are recorded; neither contract is saved. Removed 2026-09-01
  along with 44 derived collections and the artifacts derived from that spec.
- **api.tec.mx no longer exists.** The gated institutional API developer portal — the one surface
  that was the institution's own API programme, carrying named products such as *Boleta de
  Calificaciones del Alumno*, *Gestión de Estudiantes* and *Gestión de Capital Humano* — returns
  **NXDOMAIN** on 8.8.8.8, 1.1.1.1 and 9.9.9.9 as of 2026-09-01, while still being indexed by search
  engines. Its pointers were removed as dead.
- **The identity surface is the real find.** Two institution-operated SAML 2.0 IdPs on the
  institution's own registrable domains (fs.itesm.mx, amfs.tec.mx) plus a Shibboleth SP in front of
  RITEC. All three publish machine-readable metadata with no credential required.
- **RITEC is reachable again.** The June profile recorded a 403 and could not confirm the OAI-PMH
  endpoint. The human UI does sit behind an Anubis bot challenge, but `/server/api` and
  `/server/oai/request` answer 200; the old `/oai/request` path 301-redirects to the DSpace 7+ path.
- See [review.yml](review.yml) for per-URL verification status.

## Maintainers

- Kin Lane — kin@apievangelist.com
