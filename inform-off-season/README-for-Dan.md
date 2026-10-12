# Off-season landing page (informapp.com.au/off-season)

## How to launch it

1. Unzip, then copy everything inside the `inform-off-season` folder into the root of the `inform` repo. It only adds new files:
   - `off-season/index.html` (the page)
   - `assets/off-season/` (shoot photos, share image, app screenshots)
   - `assets/off-season/logos/` (the four club logos, hosted in the repo)
2. Commit and push to main. Vercel deploys it as usual.
3. Check it at https://www.informapp.com.au/off-season (phone and desktop).

Nothing that's already live gets changed. The page also uses files that must already be in the repo: `assets/landing-v2/hero-background.jpg`, `hero-video.mp4`, `hero-video-poster.jpg`, `physio-treatment.jpg`, plus `favicon.png`, `manage.html` and `subscribed.html`.

## Images

- App screenshots (`app-strength.webp`, `app-progress.webp`) are the original 1938x2460 files, untouched. The page shows them at their native ratio, so they are never cropped or stretched.
- Club logos are shown in full colour on light chips, each scaled to fit with its own ratio preserved. The Cockburn City file only had its empty margin trimmed.
- `app-goals.webp` and `strike-low.jpg` are in the folder but not used on the page yet.

## Before ads go live

- **Checkout plan.** The "Claim your spot" button uses the existing `three_month` plan ($499) on backend.informapp.com.au. That plan renews every quarter and has a "2 weeks FREE" trial on the homepage. The off-season program should be a one-off $499. If that needs a new plan in Stripe or the backend, change one line: `plan: 'three_month'` in the `OFFER` block near the bottom of `off-season/index.html`.
- **Deadline.** A countdown runs to 31 October 2026, end of day Perth time. After that the page switches to "Intake closed" on its own.
- **Club logos.** Confirm the clubs are happy for their logos to be used in paid ads.
- **Messaging screenshot.** The "Your physio is one message away" row runs text-only because no messaging screenshot was supplied. To add one, follow the comment above that row in `off-season/index.html`.
- **To swap in later:** the VSL video (the `vslVideo` element, currently the homepage video), and the GA and Meta Pixel snippets (where it says TRACKING in the head).
