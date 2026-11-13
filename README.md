# Aveno To-Do – Privacy Policy

Public privacy policy for **Aveno To-Do** (`com.aveno.todo`), an offline-first Android task manager by Aveno.

**Live page:** https://narayanaswamipaidipalli.github.io/aveno-todo-privacy/

This is the URL to use in the Google Play Console listing, in the AdMob account, and in the app's Settings screen.

## What is here

| File | Purpose |
| --- | --- |
| `index.html` | The privacy policy (single page, no scripts) |
| `style.css` | Styles (light theme, responsive, print-friendly) |
| `favicon.svg` | Aveno check-mark icon |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |

The site is plain HTML and CSS. It has no JavaScript, cookies, trackers, web fonts or build step, and a Content-Security-Policy meta tag blocks scripts and third-party resources.

## Hosting

GitHub Pages, deployed from the `main` branch, `/ (root)` folder, HTTPS enforced. Every push to `main` republishes the page within a minute or two.

## Updating the policy

1. Edit `index.html`.
2. Change the "Last updated" date near the top (both the visible text and the `datetime` attribute).
3. Commit and push to `main`.
4. Open the live page and confirm the change is visible.

The contact address appears in three places in `index.html` (sections 2, 15 and 17). Change all three together.

## What the policy was checked against

The policy describes the app as it existed in the Android source on 13 November 2026:

| Area | State of the app |
| --- | --- |
| Task storage | Room database in app-private storage; no login, backend, Firebase or sync |
| Preferences | Jetpack DataStore, on device |
| Android Auto Backup | Disabled (`android:allowBackup="false"`) |
| Export / restore | User-initiated, unencrypted JSON through the Android file picker |
| Ads | Google Mobile Ads SDK 25.1.0, banner only, Home and Lists screens, user can switch off |
| Consent | Google User Messaging Platform SDK 4.0.0; ads requested only after the consent check |
| Analytics / crash reporting | None added by the app |
| Reminders | Local notifications through WorkManager; no push server |
| App permissions | `INTERNET`, `ACCESS_NETWORK_STATE`, `POST_NOTIFICATIONS` |
| Permissions merged from libraries | `AD_ID`, `ACCESS_ADSERVICES_AD_ID`, `ACCESS_ADSERVICES_ATTRIBUTION`, `ACCESS_ADSERVICES_TOPICS`, `WAKE_LOCK`, `FOREGROUND_SERVICE` |
| Audience | General audience, not directed to children under 13 |

## Recheck before every release

The policy must be updated before a release ships if any of these change:

- A new SDK or library that sends data off the device (analytics, crash reporting, ad mediation, sign-in, cloud sync).
- A new Android permission, including ones merged in by a library. Compare against the merged **release** manifest, not only `AndroidManifest.xml`.
- A new ad format or ad placement, or a different ad network.
- A Google Mobile Ads or UMP SDK upgrade. Compare with Google's current [data disclosure](https://developers.google.com/admob/android/privacy/play-data-disclosure).
- Any change to backup, export, restore or deletion behaviour, or enabling Android Auto Backup.
- A change to the intended audience or to child-directed ad settings.
- A change of developer name or privacy contact address.

The Google Play Data safety form and this policy must always say the same thing.

## Contact

Privacy questions: see the contact section of the live policy.
