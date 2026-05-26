# vestimentum-site

Public static site for [vestimentum.app](https://vestimentum.app) —
landing page + bilingual legal docs (KVKK/GDPR Privacy Policy +
Terms of Service in TR + EN).

Built with Jekyll, hosted on GitHub Pages, custom domain via
`CNAME` + DNS records at the registrar.

## Stack

- **Jekyll 3.x** (auto-built by GitHub Pages on push)
- **Fraunces** (serif headings) + **Inter** (sans body), loaded via
  Google Fonts at runtime — no asset pipeline
- **No theme** — bespoke layout in `_layouts/default.html` keeps
  the page <50 KB on first load
- **Pretty URLs** via `permalink: pretty` so `/legal/privacy_policy_tr/`
  resolves to `legal/privacy_policy_tr/index.html`. These paths
  match the URLs the Vestimentum mobile app hardcodes in
  `core/legal/legal_urls.dart` (private repo).

## Local preview

```bash
# Requires Ruby + bundler installed
gem install jekyll
jekyll serve --watch
# Opens at http://127.0.0.1:4000
```

You can also just push and let GitHub Pages build it — the live
preview pipeline reloads automatically after each push.

## Deploy

GitHub Pages is configured in **Settings → Pages** to deploy from
the `main` branch root. Push to `main`, wait ~30-60 seconds for
Jekyll to rebuild, refresh `https://vestimentum.app`.

## Custom domain

`CNAME` (single line: `vestimentum.app`) is committed at the root.
The DNS records for the apex + `www` subdomain are documented in
the main repo at `vestimentum/DNS_SETUP.md` — copy the four A
records + the www CNAME to your registrar's DNS panel.

GitHub Pages auto-provisions a Let's Encrypt SSL cert once the
DNS records propagate (typically 15-30 minutes). After that, enable
"Enforce HTTPS" in Settings → Pages.

## Legal docs — source of truth

Canonical Markdown lives in the **private main repo** at
`vestimentum/legal/*.md`. Copies in this repo's `legal/` directory
have a Jekyll frontmatter block prepended for layout + permalink
routing.

**Sync workflow** when legal docs change in main repo:

```bash
# From the parent directory containing both repos
for f in privacy_policy_tr privacy_policy_en terms_of_service_tr terms_of_service_en; do
  # Keep the frontmatter (top 7 lines), replace the body below.
  head -n 7 vestimentum-site/legal/$f.md > vestimentum-site/legal/$f.tmp
  cat vestimentum/legal/$f.md >> vestimentum-site/legal/$f.tmp
  mv vestimentum-site/legal/$f.tmp vestimentum-site/legal/$f.md
done
cd vestimentum-site
git add legal/ && git commit -m "sync: legal docs from main repo" && git push
```

Manual until / unless we set up a GitHub Action that pulls from
the private repo on a schedule.

## Pre-launch checklist

Before announcing the site publicly:

- [ ] Replace placeholder email addresses in legal/*.md
      (`privacy@vestimentum.app`, `support@vestimentum.app`,
      `legal@vestimentum.app`). Either set up email forwarding at
      your domain registrar so those addresses route to your real
      inbox, or replace them outright with `oguzcanozupek@gmail.com`.
- [x] Yargı yeri — "İzmir Mahkemeleri" finalized 2026-05-26.
      No further change.
- [ ] Lawyer review (₺3-7K, 1-2 weeks). Pre-launch blocker.
- [ ] Effective date in each legal/*.md: update to actual launch
      day.
- [ ] If incorporated, replace "Oğuzcan Özüpek tarafından
      geliştirilmektedir" with the corporate entity name + MERSIS
      no + registered address.
- [ ] After deployment, smoke-test all four legal URLs from the
      mobile app: Profile → Hukuki / Legal → tap each row, verify
      `url_launcher` opens the right URL.
- [ ] Once on Play Store / App Store, paste the privacy URL into
      the listing's "Privacy Policy" field.
