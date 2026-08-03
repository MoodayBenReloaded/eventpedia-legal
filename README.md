# EVENTPEDIA — legal pages

Public source for the Privacy Policy and Terms of Service linked from the
EVENTPEDIA app (Settings → About) and from eventpedia.app.

Deliberately a **separate public repo**: the app repo is private and contains
migrations, environment files and partner supply data. GitHub Pages needs a
public repo on the free plan, and legal text changes on legal timelines rather
than release timelines — so it does not belong in the app's deploy path.

- Served by GitHub Pages from `/docs` on `main`.
- Hand-written HTML + one stylesheet. No build, no dependencies, no external
  requests — a page about not leaking your requests should not call a CDN.

> **Draft.** Pages still carry `[FILL: …]` placeholders for the legal entity,
> address and contact email, and are `noindex` until those are filled. Do not
> link them publicly or submit them to App Store review in this state.
