# SSL Control Baseline — 2026-07-30

## Governing sources

1. **Website source:** `docsage420-stack/sage-systems-lab`
2. **Production branch:** `main`
3. **Hosting project:** Netlify `sage-systems-lab`
4. **Production domain:** https://sagesystemslab.net/
5. **Commerce source:** https://www.etsy.com/shop/SageSystemsLab
6. **Canonical public product data:** `data/products.json`

The Netlify production project is linked to GitHub `main`. Production changes must flow through a branch and reviewed pull request. Manual production uploads are not the governing workflow.

## Verified public operating state

- Six active Etsy listings
- Two sales
- One five-star review
- Website and shop are public
- Website is a static Netlify deployment
- No build system, test suite, forms, or serverless functions
- Each website product now has a direct Etsy listing link on this branch

## Control rules

- Do not use OneDrive to synchronize repositories.
- Do not maintain competing product facts in page copy, prompts, and spreadsheets.
- Update `data/products.json` first when a listing ID, format, compatibility claim, or product status changes.
- Product claims must be product-specific.
- Pricing is intentionally excluded from canonical data because Etsy controls the live price.
- Never publish financial outcomes as guarantees.
- Do not claim all products are offline; format and device behavior vary.
- Merge website changes only after link, markup, mobile, and claim validation.

## Immediate backlog

1. Merge direct product links and canonical catalog.
2. Build one search-indexable landing page per active product.
3. Add a privacy-compatible measurement plan before introducing analytics.
4. Select one flagship product using listing-level Etsy visits, favorites, orders, and revenue.
5. Build a free functional demo or guided preview for the flagship.
6. Create a repeatable listing-content package from canonical product data.
7. Add automated link and structured-data validation.
8. Reconcile the newer Fable 5 and Opus 4.8 SSL work against this baseline before merging either implementation.

## Acceptance tests for the next website release

- All six product links resolve to the intended Etsy listing.
- Structured data uses the same listing URLs as visible buttons.
- Homepage content matches active product status.
- No product claim is broadened to the full catalog.
- Keyboard focus remains visible.
- Layout works at 375 px, 768 px, and 1440 px widths.
- Netlify preview deploy succeeds before production merge.
