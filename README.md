# Tiny Thief: Castle Heist — app homepage

Static app homepage, privacy policy, support page, and AdMob app-ads.txt, following the Paper Boat site structure with a dark castle palette. No build tools, dependencies, tracking scripts, or external fonts are required.

## Preview

Run `python3 -m http.server 8080` in this folder, then open http://localhost:8080.

## GitHub Pages

Publish this repository using GitHub Pages (Settings → Pages → Deploy from a branch → main → / root). The expected URL is https://weidinger-c.github.io/Tiny-Thief-Castle-Heist-App/ once Pages is enabled and these files are pushed. No deployment has been performed as part of creating the files.

- Marketing URL: site root
- Support URL: support.html
- Privacy URL: privacy.html

The App Store listing URL is not yet configured. Once the app's public listing is known, add its real link to the homepage; there is deliberately no placeholder download button.

## Advertising verification

app-ads.txt uses the AdMob publisher ID pub-6235626639390894. AdMob looks for this file at the root of the developer website domain. A GitHub Pages project path alone may not satisfy that lookup: also serve this same file at https://weidinger-c.github.io/app-ads.txt (via the user-site repository), or use a custom domain with this file at its root. Configure the published developer website in App Store Connect and verify its crawl status in AdMob.

## Assets and content

icon.png and assets/castle.webp reuse the game's own artwork (app icon and menu background). assets/sneak.webp (heist 4, Smoke & Mirrors) and assets/alarm.webp (heist 20, Lockdown) are actual English gameplay captures. Images are local and optimized.

Privacy and support text are based on the current app implementation: 72 heists in 9 wings, local-only saves (no account, no iCloud, no purchases), Google AdMob interstitials between heists (not after the first heist, not on retries, at most every 45 s), the UMP consent message before App Tracking Transparency, non-personalised ads without tracking permission, and Privacy choices in Settings when Google requires it. Recheck these pages when app behavior or SDK data practices change.
