# avna ⚓

**GDPR cookie consent your coding agent can install in one API call.**

A one-line banner, consent records with signed receipts, hosted in France. Free up to 200 consents per month, then €9.99/month per website.

```html
<!-- one line, in your <head> -->
<script src="https://api.getavna.com/avna.js" data-site="cs_…"></script>
```

```sh
# or, for an agent — no account needed:
curl -X POST https://api.getavna.com/v1/sites \
  -d '{"name":"My site","domain":"example.com","country":"fr"}'
```

**[getavna.com](https://www.getavna.com)** · [Free site scanner](https://www.getavna.com/scan) · [Subprocessors & DPA](https://www.getavna.com/dpa)

## Open source

| Repository | What | License |
|---|---|---|
| [`avna`](https://github.com/getavna/avna) | The banner SDK — < 5 KB gzipped, zero dependencies | MIT |
| [`jurisdictions`](https://github.com/getavna/jurisdictions) | Cookie-consent doctrine for 56 jurisdictions, sourced from the national authorities | CC-BY-4.0 |

The SDK you drop on your site and the doctrine it applies are both open — read them and fork them. The hosted backend keeps your records in France; the self-hostable backend is opening next. The SDK, CLI, API, a stdio MCP server and per-site `consent.txt` are already live — a formal `consent.txt` spec for agent-mediated consent is next.

---

avna is a compliance tool, not legal advice. Designed to align with EDPB and national authority guidance (CNIL, Garante, AEPD, …) — never marketed as “guaranteed compliance”.
