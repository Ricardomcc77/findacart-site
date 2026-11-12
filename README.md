# FindACart public website

Informational company and product website for **FindACart LLC**, served at **https://findacart.com** by the existing GitHub Pages configuration in `Ricardomcc77/findacart-site`.

Plain HTML and CSS; no build, JavaScript runtime, third-party fonts, analytics scripts, API calls, or form service. Contact actions open the visitor’s email app. The product is still in development; this website does not register accounts or accept orders.

## Pages and assets

- `/` — product story, current app screenshots, company information, launch FAQ, and company email.
- `/privacy/`, `/terms/` — existing page body wording retained; shared navigation and styling updated.
- `styles.css` — shared responsive layout, focus states, print styles, and reduced-motion behavior.
- `assets/` — original generated grocery image, responsive WebP encodings, a JPEG link preview, current app screenshots, and provenance.
- `fonts/` — existing self-hosted fonts and SIL Open Font Licenses.
- `CNAME` — existing custom domain, `findacart.com`; keep this file when deploying.
- `sitemap.xml` and `robots.txt` — public route discovery.

The two product previews use the current Svelte web app with synthetic sample data: the planner’s dinner summary and a focused view of the shopping list’s Produce aisle. Both details are direct 2x screenshots of the app’s rendered elements, with no position-dependent CSS crop. The source images are unretouched, and the caption identifies sample data. They show an unreleased product, not a publicly available service. There are no retailer logos, store badges, testimonials, user counts, pricing promises, or announced partnerships.

## Preview and check

From this directory:

```sh
python3 -m http.server 8765 --bind 127.0.0.1
```

Open http://127.0.0.1:8765. Use an HTTP server: root-relative asset links intentionally target the domain root and will not work by double-clicking an HTML file.

Before publishing, check all three pages at phone and desktop widths, keyboard navigation and focus, the primary product anchor, FAQ disclosure controls, mailto destinations, and policy links. Verify there are no missing images/fonts or horizontal overflow. The FAQ and navigation work without JavaScript. No backend or app build is needed for this separate repository.

## Content maintenance

- Update launch status only when downloads or web access are actually available.
- Keep company name and contact details consistent with the actual business and enrollment applications.
- Do not promise grocery ordering, checkout, prices, availability, or fulfillment that is not integrated and verified.
- Changes to shared navigation must be reflected in all three HTML pages. Keep canonical URLs and the sitemap in sync when adding routes.
- Policy wording remains owned by the product/legal source; review substantive changes separately.

## Purpose

The site introduces FindACart and FindACart LLC so visitors and application reviewers can understand the business and product. It is intended to support website verification for developer and affiliate applications, including Instacart and Walmart, without advertising partnerships or inviting sales discussions. Program acceptance is determined by the provider.

## Publishing

This change is prepared for the existing GitHub Pages repository and hosting setup. Publishing requires updating its configured source branch; do not upload it into the application repository or change DNS. Keep `CNAME`, existing policy routes, and the domain’s HTTPS configuration. After publishing, verify the public homepage, policy routes, and HTTPS on the custom domain.

The prelaunch site has no Support page. When applying this source to the existing repository, include the deletion of the previously tracked `support/index.html`; copying only the ZIP’s remaining files would leave that old page behind.
