# EVENTPEDIA — legal pages

Public source for the Privacy Policy and Terms of Service, in English and
Thai, linked from the EVENTPEDIA app (Settings → About) and from
eventpedia.app.

| Page | English | Thai |
|---|---|---|
| Privacy Policy | `docs/privacy.html` | `docs/privacy-th.html` |
| Terms of Service | `docs/terms.html` | `docs/terms-th.html` |
| Contact and support (App Store Support URL) | `docs/index.html` (both languages) | |

The app repo keeps an identical copy in its own `docs/`; change both
together.

Deliberately a **separate public repo**: the app repo is private and contains
migrations, environment files and partner supply data. GitHub Pages needs a
public repo on the free plan, and legal text changes on legal timelines rather
than release timelines — so it does not belong in the app's deploy path.

- Served by GitHub Pages from `/docs` on `main`.
- Hand-written HTML + one stylesheet. No build, no dependencies, no external
  requests — a page about not leaking your requests should not call a CDN.

> **Draft.** The pages carry five marked placeholders: `[FILL: COMPANY NAME]`,
> `[FILL: REGISTERED ADDRESS]`, `[FILL: CONTACT EMAIL]`,
> `[FILL: DATA PROTECTION CONTACT]` and `[FILL: EFFECTIVE DATE]`, and are
> `noindex` until those are filled. After filling them, remove the noindex
> comment and meta line from every page and check that a search for `[FILL`
> finds nothing. Do not link the pages publicly or submit them to App Store
> review before that.
