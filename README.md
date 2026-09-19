# Inform website updates — apply these 3 changes

1. Replace `index.html` at the repo root with the one in this zip.
2. Delete `form.html` from the repo (no longer used/linked anywhere).
3. Delete `landing.html` from the repo (unused standalone ad-campaign page).

Then commit and push — Vercel will auto-deploy.

## Summary of what changed in index.html

- All top-level CTA buttons (nav, hero, final CTA) now say "Sign up now" and link to
  #pricing (the live Stripe checkout), instead of the old waitlist form.
- "The judgment stays human." section is now a 2-column layout: copy left, photo right
  (16px rounded corners).
- "Human in the loop" feature row now uses the new phone screenshot image.
- Added a simple contact form above the footer (Name, Email, Phone, Message), submitting
  via the same Formspree endpoint the old form used.
