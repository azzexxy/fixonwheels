# Fix on Wheels

Website for Fix on Wheels, a mobile phone and laptop repair van in Ghent (Rune Waltniel & Lothar Van Cauwenbergh).

Everything is in one file: `index.html`. Open it in a browser, no build step.

The 3D van on the landing page is drawn with three.js, loaded from the jsDelivr CDN by the module script at the bottom of `index.html`. If it can't load, the rest of the page still works.

## Before going live

At the top of the `<script>` in `index.html`, edit `CONFIG`:

- `bookingEmail` – where booking requests are sent (the form opens the visitor's email app)
- `tiktok`, `instagram` – your profile links

Prices live in the `PRICES` object and time slots in `WEEKDAY_SLOTS` / `SAT_SLOTS`. The "taken" slots are simulated; connect a real booking tool (Calendly, Cal.com, a form backend) when you're ready.

## Host it free

GitHub: Settings → Pages → Deploy from branch `main`, folder `/ (root)`.
