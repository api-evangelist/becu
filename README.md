# BECU (becu)

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
