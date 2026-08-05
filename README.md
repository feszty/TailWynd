# Tailwynd Website

Static website for Tailwynd, ready for GitHub Pages. Adapted from the
IntroCard site template.

## Deploy

1. Upload all files and folders to a `tailwynd` GitHub repository.
2. Go to Settings > Pages.
3. Select `Deploy from a branch`, branch `main`, folder `/root`.
4. Set the custom domain (the `CNAME` file currently says `tailwynd.autos` —
   already set).
5. Configure DNS with your domain registrar.
6. Enable Enforce HTTPS after DNS has propagated.

## Before launch

- `CNAME` and the `support@tailwynd.autos` addresses in all three pages
  assume the tailwynd.autos domain — update both if you register a
  different one.
- index.html and support.html currently link the public TestFlight beta
  (testflight.apple.com/join/KXeU5cnZ). At App Store launch, replace with
  the real `https://apps.apple.com/app/idXXXXXXXXXX` link.
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
