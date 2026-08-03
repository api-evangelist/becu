# BECU (becu)

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

BECU (Boeing Employees' Credit Union) is a member-owned, not-for-profit state-chartered credit union founded in 1935 and headquartered in Tukwila, Washington (NMLS ID 490518). Originally serving Boeing employees, it is today one of the largest credit unions in the United States, offering consumer and business deposit accounts, lending, mortgages, and investment services.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/becu/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/becu/refs/heads/main/apis.yml)

## Open Finance / API Posture

BECU exposes **no public first-party developer API and no public developer portal**. Probes of the usual developer hostnames confirmed this:

- `developer.becu.org` — does not resolve (no DNS record)
- `developers.becu.org` / `apis.becu.org` — resolve to F5 Distributed Cloud infrastructure but reset the connection with no public TLS content
- `api.becu.org` — an F5 Distributed Cloud gateway host returning HTTP 403 (gated internal/partner gateway, not a documented public API)
- `www.becu.org/api-developer` — HTTP 404

This is the honest and typical reality for a US credit union. US open finance is **voluntary and fragmented** — there is no single mandated open-banking contract. BECU's digital banking runs on established core and fintech vendors (FIS / Client Point, LPL Account View, ICE/Ellie Mae for mortgage), and consumer-permissioned data sharing for third-party fintech apps is intermediated through **data aggregators** (Plaid / MX / Finicity / Akoya) rather than a self-serve BECU API. The emerging **CFPB Section 1033** Personal Financial Data Rights rule is the framework expected to shape BECU's future data-access posture; no first-party 1033 or FDX data-access API is publicly documented at this time.

## Tags

- Financial Services
- Banking
- United States
- Credit Union
- Open Finance
- Data Aggregation
- CFPB 1033

## Timestamps

- **Created:** 2026-07-23
- **Modified:** 2026-07-23

## APIs

No public developer APIs are documented. See the Open Finance / API Posture section above.

## Common Properties

- [Website](https://www.becu.org/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
