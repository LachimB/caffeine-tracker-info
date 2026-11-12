# Caffeine Tracker — public information

Public information website for the Caffeine Tracker Android app, maintained by [LachimB](https://github.com/LachimB). This repository contains only the independently authored static website; it does not contain the Android source, APKs, app records, backups, credentials, or private repository history.

## Published pages

- [Application home page](https://lachimb.github.io/caffeine-tracker-info/)
- [Privacy policy](https://lachimb.github.io/caffeine-tracker-info/privacy.html)
- [Terms of service](https://lachimb.github.io/caffeine-tracker-info/terms.html)

## Hosting and editing

GitHub Pages publishes the root of the `main` branch. `.nojekyll` disables Jekyll processing. Edit the three HTML files and shared assets directly; there is no build step, JavaScript, analytics, external font, or dependency install. For a local preview, run `python3 -m http.server 8765` from this directory.

Keep all links relative so the website also works under a custom domain. If changing the public domain, update the canonical URLs in the three HTML files and these links. Keep the privacy policy accurate when app data practices change.

## Google OAuth branding setup

Use the published home page, privacy policy and terms URLs in Google Auth Platform → Branding. The app name should match **Caffeine Tracker**. Set the existing developer-controlled support email separately in the Google console; no personal email is published by this website.

Google also requires domain ownership verification for brand review. A deployed GitHub Pages URL alone does not prove that verification or guarantee approval. Use Google Search Console with an owner/editor of the OAuth project. If Google cannot accept verification for the hosted subdomain, configure a domain you own for GitHub Pages and update all three URLs. Add only the corresponding accepted top private domain in Authorized domains; do not use `github.com` or a repository path as your app domain. Do not create a new OAuth client or expand API scopes just to publish these pages.

Official guidance: [brand verification](https://developers.google.com/identity/protocols/oauth2/production-readiness/brand-verification), [OAuth policy compliance](https://developers.google.com/identity/protocols/oauth2/production-readiness/policy-compliance).

## Support

[Open a support issue](https://github.com/LachimB/caffeine-tracker-info/issues) for general questions. Issues are public. Never upload journal data, backups, account details, credentials or screenshots containing personal information.
