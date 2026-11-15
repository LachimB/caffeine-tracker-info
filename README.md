# Caffeine Tracker — public information

Public information website for the Caffeine Tracker Android app, maintained by [LachimB](https://github.com/LachimB). This repository contains only the independently authored static website; it does not contain the Android source, APKs, app records, backups, credentials, or private repository history.

## Published pages

- [Application home page](https://lachimb.github.io/caffeine-tracker-info/)
- [Privacy policy](https://lachimb.github.io/caffeine-tracker-info/privacy.html)
- [Terms of service](https://lachimb.github.io/caffeine-tracker-info/terms.html)

## Feature availability

The latest numbered release uses favourites-based logging and native date/time pickers. The unified drink catalogue, named sizes, espresso-equivalent recipes and optional AI estimates described below are development features awaiting a later numbered release.

## App features described here

The app records caffeine intake locally, with one editable drink catalogue, estimated starter recipes, History corrections, configurable latest-action Undo, statistics and optional Google Drive exports/backups. Recipes support milligrams or espresso equivalents, optional serving prompts, arbitrary volumes and named sizes with independent caffeine amounts or espresso counts. Existing recipes and historical records keep their recorded details through upgrades, edits and archiving. Legacy linked-choice summaries remain available.

Optional OpenAI caffeine estimates require a user-provided API key. The disabled wand becomes available after key setup and when the amount is blank. Explicit requests send only a drink name and optional reference/serving volume; users review the estimate before use. The key is encrypted on-device and excluded from journal exports and backups. Provider processing and possible API charges are described in the privacy policy and terms.

## Hosting and editing

GitHub Pages publishes the root of the `main` branch. `.nojekyll` disables Jekyll processing. Edit the three HTML files and shared assets directly; there is no build step, JavaScript, analytics, external font, or dependency install. For a local preview, run `python3 -m http.server 8765` from this directory.

Keep all links relative so the website also works under a custom domain. If changing the public domain, update the canonical URLs in the three HTML files and these links. Keep the privacy policy accurate when app data practices change.

## Google OAuth branding setup

Use the published home page, privacy policy and terms URLs in Google Auth Platform → Branding. The app name should match **Caffeine Tracker**. Set the existing developer-controlled support email separately in the Google console; no personal email is published by this website.

Google also requires domain ownership verification for brand review. A deployed GitHub Pages URL alone does not prove that verification or guarantee approval. Use Google Search Console with an owner/editor of the OAuth project. If Google cannot accept verification for the hosted subdomain, configure a domain you own for GitHub Pages and update all three URLs. Add only the corresponding accepted top private domain in Authorized domains; do not use `github.com` or a repository path as your app domain. Do not create a new OAuth client or expand API scopes just to publish these pages.

Official guidance: [brand verification](https://developers.google.com/identity/protocols/oauth2/production-readiness/brand-verification), [OAuth policy compliance](https://developers.google.com/identity/protocols/oauth2/production-readiness/policy-compliance).

## Support

[Open a support issue](https://github.com/LachimB/caffeine-tracker-info/issues) for general questions. Issues are public. Never upload journal data, backups, account details, credentials or screenshots containing personal information.
