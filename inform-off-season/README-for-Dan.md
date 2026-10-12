# Off-season landing page (informapp.com.au/off-season)

## How to launch it

1. Copy everything inside the `inform-off-season` folder into the root of the `inform` repo. It only adds new files:
   - `off-season/index.html` (the page)
   - `assets/off-season/` (the shoot photos and the share image)
2. Commit and push to main. Vercel deploys it as usual.
3. Check it at https://www.informapp.com.au/off-season

Nothing that's already live gets changed. The page also uses a few files that are already in the repo: the homepage video, the hero background and the physio photo in `assets/landing-v2/`, plus `favicon.png`, `manage.html` and `subscribed.html`.

## Before ads go live

- **Checkout plan.** The "Claim your spot" button uses the existing `three_month` plan ($499) on backend.informapp.com.au. That plan renews every quarter and has a "2 weeks FREE" trial on the homepage. The off-season program should be a one-off $499. If that needs a new plan in Stripe or the backend, change one line: `plan: 'three_month'` in the `OFFER` block near the bottom of `off-season/index.html`.
- **Deadline.** A countdown runs to 31 October 2026, end of day Perth time. After that the page switches to "Intake closed" on its own.
- **Club logos.** The "Trusted by" strip loads from inform-physio.com.au. If that site blocks it, the strip hides itself. It's safer to copy the logos into the repo.
- **To swap in later:** the VSL video (the `vslVideo` element, currently the homepage video), the 3 app screenshots (marked PLACEHOLDER), and the GA and Meta Pixel snippets (where it says TRACKING in the head).
