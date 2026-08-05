# Tailwynd Website

Static website for Tailwynd, ready for GitHub Pages. Adapted from the
IntroCard site template.

## Deploy

1. Upload all files and folders to a `tailwynd` GitHub repository.
2. Go to Settings > Pages.
3. Select `Deploy from a branch`, branch `main`, folder `/root`.
4. Set the custom domain (the `CNAME` file currently says `tailwynd.app` —
   change it to whatever domain you register).
5. Configure DNS with your domain registrar.
6. Enable Enforce HTTPS after DNS has propagated.

## Before launch

- `CNAME` and the `support@tailwynd.app` addresses in all three pages
  assume the tailwynd.app domain — update both if you register a
  different one.
- The App Store buttons say "Coming soon" — replace with the real
  `https://apps.apple.com/app/idXXXXXXXXXX` link on index.html and
  support.html at launch.
- The screenshots section in `index.html` is commented out. Drop App
  Store screenshots into `/images` as `tailwynd_01_plan.png` …
  `tailwynd_04_report.png` (or edit the filenames) and un-comment it.
- `/images` still contains the old IntroCard screenshots
  (`appstore_*.png`) and `/videos` the IntroCard demo — unreferenced
  now; delete them before publishing.
- `images/AppIcon.png` is the Tailwynd app icon (also used as favicon
  and nav logo).

## Privacy note

`privacy.html` describes the app as shipped: no accounts, local-only
trip data, anonymous weather queries, no connected-car integration.
If the Smartcar path is ever re-enabled, update the policy BEFORE
shipping that build.
