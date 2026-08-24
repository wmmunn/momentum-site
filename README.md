# momentum-site

Product site for Momentum (Plex Music for Cars), served by GitHub Pages at
https://momentumcar.app

Plain static HTML + one stylesheet. No build step, no framework, no dependencies.
Edit a file, commit, push; Pages redeploys automatically in about a minute.

## Files

- `index.html` — landing page (the pitch; store listing links here)
- `setup.html` — requirements + the two-minute reachability test (content moved off the Play listing)
- `faq.html` — help / troubleshooting answers (expand from real support cases)
- `style.css` — shared stylesheet (dark + gold, matches the app)
- `CNAME` — tells GitHub Pages to serve at momentumcar.app (do not delete)

## Publishing (one-time setup)

1. Create a public repo named `momentum-site` on GitHub and push these files
   to `main` (files at the repo root, not in a subfolder).
2. Repo Settings → Pages → Source: "Deploy from a branch" → `main` / `/ (root)`.
3. In the same Pages settings, Custom domain: `momentumcar.app`.
   DNS is already set at Porkbun (4 A records + www CNAME), so the check
   should pass; then tick "Enforce HTTPS" once the certificate is issued
   (can take up to an hour on first setup).
4. Optional, recommended: GitHub account Settings → Pages → verified domains →
   add momentumcar.app. Prevents domain takeover if the repo is ever deleted.

## Before the site is "done" — open TODOs

Search the HTML for `TODO`:

- Play Store link on `index.html` (verify package id against the Play Console)
- Privacy policy link in all three footers (point at the existing policy,
  or move the policy into this repo)
- Support email: switch from gmail to support@momentumcar.app after setting up
  free email forwarding at Porkbun (EMAIL icon on the domain row)
- FAQ answers are drafts; expand from real tester cases

## Voice note

All copy is a working draft. Re-voice before treating any page as final,
same as any public-facing text.
