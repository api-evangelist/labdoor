# LabDoor

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

Labdoor is an independent supplement testing company. It buys top-selling vitamins, supplements, protein powders and energy drinks off retail shelves and online stores, sends samples to FDA-registered analytical laboratories for chemical analysis of active ingredients and potential contaminants, grades each product on Label Accuracy, Product Purity, Nutritional Value, Ingredient Safety and Projected Efficacy, and publishes the resulting rankings and expert reports for free. Testing is funded by retail sales and by Labdoor Enterprise certification and custom-testing services sold to manufacturers.

Backed by: 500-global, y-combinator — https://labdoor.com

## API surface

**Labdoor publishes no public API** as of 2026-07-19. Verified during the enrichment pass:

- No developer portal, API documentation, or API reference (`/developers`, `developer.labdoor.com`, `docs.labdoor.com` all absent).
- No OpenAPI/Swagger/GraphQL/AsyncAPI specification published anywhere.
- No first-party SDKs or packages on npm, PyPI, or RubyGems.
- The `github.com/labdoor` organization exists (Labdoor Inc., San Francisco, created 2015) but has **0 public repositories**.
- No `/llms.txt`, no `/.well-known/*` discovery documents, no status page, no trust center, no security.txt, and no published vulnerability disclosure program.
- `api.labdoor.com` resolves and serves an Apache default page (HTTP 403 at root, 404 on probed paths). Its CORS response headers advertise `x-api-key`, `authorization`, and `x-labdoor-captcha`, so it is the first-party web application's backend — undocumented and not offered as a public product. It is deliberately **not** recorded as an API in `apis.yml`.
- `robots.txt` disallows `/service/*`, but no `/service/*` path returned anything other than 404.

## Artifacts

| Artifact | File | Method |
|---|---|---|
| Domain security | `security/labdoor-domain-security.yml` | probed |
| Well-known probe | `well-known/labdoor-well-known.yml` | searched (none found) |
| llms.txt | `llms/labdoor-llms.txt` | generated |
