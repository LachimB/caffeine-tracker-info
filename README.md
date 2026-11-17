# Caffeine Tracker — public information

Public information website for the Caffeine Tracker Android app, maintained by [LachimB](https://github.com/LachimB). This repository contains only the independently authored static website; it does not contain the Android source, APKs, app records, backups, credentials, or private repository history.

## Published pages

- [Application home page](https://lachimb.github.io/caffeine-tracker-info/)
- [Privacy policy](https://lachimb.github.io/caffeine-tracker-info/privacy.html)
- [Terms of service](https://lachimb.github.io/caffeine-tracker-info/terms.html)

## Feature availability

The day review update adds explicit complete and caffeine-free confirmations in the day journal. Entry changes reopen affected dates, and the latest review action can be undone. An optional evening reminder is independent of caffeine targets. Existing journal entries, recipes and caffeine averages keep their meaning.

## App features described here

Journal combines current, past and future dates in one day journal, replacing the separate History screen. Use the previous/next arrows or swipe right for the previous day and left for the next, with a short transition between dates. A visible swipe hint explains the gesture. Tap the day overview for a date picker with a Today shortcut. Relative labels distinguish today, yesterday, tomorrow, history and future. A trash button beside each entry’s pen opens deletion confirmation; the existing Undo window still applies.

The app opens to Journal with logged caffeine, positive-caffeine drink count, last known observed caffeine time, optional daily target progress and correction access. An Add drink button between the overview and today’s entries opens a separate form. Saving returns to Journal with Undo; Back preserves the unfinished draft. New-entry and correction previews show the selected date’s total after saving, including both dates for a move. Unknown times and future consumption stay explicit. A deliberately selected historical draft keeps its date through navigation and restarting. These views calculate on-device without new permissions or automatic AI requests. Day review distinguishes unconfirmed, confirmed complete and confirmed caffeine-free dates. Positive caffeine blocks caffeine-free confirmation. Future dates and known future consumption must wait for explicit review; unknown times remain unknown. Entry changes reopen affected dates atomically, and Undo restores the appropriate review states. Optional evening reminders use the device time zone and existing notification permission; they never confirm a day automatically. Explicit day-status exports and full backup recovery retain review state separately from drinks and choices.

The app records caffeine intake locally, with one editable drink catalogue, estimated starter recipes, day-journal corrections, configurable latest-action Undo, statistics and optional Google Drive exports/backups. Recipes support milligrams or espresso equivalents, optional serving prompts, arbitrary volumes and named sizes with independent caffeine amounts or espresso counts. Existing recipes and historical records keep their recorded details through upgrades, edits and archiving.

Optional OpenAI caffeine estimates require a user-provided API key. The disabled wand becomes available after key setup and when the amount is blank. Explicit requests send only a drink name and optional reference/serving volume; users review the estimate before use. The key is encrypted on-device and excluded from journal exports and backups. Provider processing and possible API charges are described in the privacy policy and terms.

The “When you drink caffeine” card shows your typical last-drink time and whether it has moved earlier or later than the previous period, in minutes or hours. The typical time averages complete, finished days with every caffeine drink timed in one time zone. A compact selector lets you browse 7-day, 28-day or calendar-week periods. If you enable a personal cutoff, the card also shows the amount logged at or after it, using recorded local clocks. Timing details explains the included records and comparisons, with weekday/weekend averages and first and last caffeine by date. Trends match complete, fully timed days on the same weekdays in compatible time zones. Optional current-day timing detail remains available in Journal. These are observations of your log, not remaining-caffeine estimates or sleep predictions.

Timing calculations stay on-device. Optional timing settings are included in full backups, with no new permission or automatic AI request. Existing exports and journal history retain their meaning.

Home widgets show today’s logged caffeine and caffeinated-drink count. Choose a drink from the same catalogue for each widget, using Widget setup or Settings → Home widgets. Enlarge an existing small widget to show recipe and setup actions; small widgets retain the read-only summary and tap-to-open-Journal route. Logging opens an app review and saves only when you confirm. Prompted serving sizes are resolved first, including sizes with their own caffeine dose and no volume. Use the shared Undo window or open Journal to correct a saved record.

Widget references and unfinished reviews are included in full backups. Refreshing or configuring a widget never logs a drink. No additional permission or automatic AI request is introduced.

## Hosting and editing

GitHub Pages publishes the root of the `main` branch. `.nojekyll` disables Jekyll processing. Edit the three HTML files and shared assets directly; there is no build step, JavaScript, analytics, external font, or dependency install. For a local preview, run `python3 -m http.server 8765` from this directory.

Keep all links relative so the website also works under a custom domain. If changing the public domain, update the canonical URLs in the three HTML files and these links. Keep the privacy policy accurate when app data practices change.

## Google OAuth branding setup

Use the published home page, privacy policy and terms URLs in Google Auth Platform → Branding. The app name should match **Caffeine Tracker**. Set the existing developer-controlled support email separately in the Google console; no personal email is published by this website.

Google also requires domain ownership verification for brand review. A deployed GitHub Pages URL alone does not prove that verification or guarantee approval. Use Google Search Console with an owner/editor of the OAuth project. If Google cannot accept verification for the hosted subdomain, configure a domain you own for GitHub Pages and update all three URLs. Add only the corresponding accepted top private domain in Authorized domains; do not use `github.com` or a repository path as your app domain. Do not create a new OAuth client or expand API scopes just to publish these pages.

Official guidance: [brand verification](https://developers.google.com/identity/protocols/oauth2/production-readiness/brand-verification), [OAuth policy compliance](https://developers.google.com/identity/protocols/oauth2/production-readiness/policy-compliance).

## Support

[Open a support issue](https://github.com/LachimB/caffeine-tracker-info/issues) for general questions. Issues are public. Never upload journal data, backups, account details, credentials or screenshots containing personal information.
