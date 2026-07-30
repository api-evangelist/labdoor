# LabDoor

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
