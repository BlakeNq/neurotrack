# NEUROTRACK

A responsive, local-first medication and caffeine logging PWA prototype. Built with plain HTML/CSS/JavaScript and IndexedDB. No accounts, server, tracking scripts, or external dependencies.

## Deploy to GitHub Pages
1. Create a GitHub repository (public for GitHub Pages on a free account).
2. Upload the **contents** of this folder to the repository root.
3. Open **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, branch `main`, folder `/ (root)`, then Save.
4. Open the Pages URL. To use your domain, set **Settings → Pages → Custom domain**, then configure DNS as instructed by GitHub and enable HTTPS.
5. On iPhone, open the site in Safari → Share → **Add to Home Screen**.

## What works
- Local IndexedDB persistence, export/import JSON, and reset
- Recurring weekly schedules and per-strength whole-week inventory forecasting
- Dose taken/skipped/undo with stock updates and logged time
- Caffeine logs and relative, illustrative time curves
- Daily check-ins, sleep, focus, side effects and notes
- Responsive dark UI and offline service-worker cache

## Prototype limitations
- The curves are illustrative only, **not clinically validated pharmacokinetic models**. They must not guide medication or caffeine dosing.
- No push notifications or actual Discord webhook sends. These require an authenticated backend, permissions, and secure server-side secret management.
- The backup JSON is **not encrypted**. Treat it as sensitive health data.
- School and bedtime settings are saved but not yet drawn as graph overlays.
- Future calendar dates show the repeating plan, not the complete-week stock allocation. The forecast panel applies the complete-week policy.
- This app is not a medical device and does not replace professional guidance.
