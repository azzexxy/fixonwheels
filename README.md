# Fix on Wheels

Website for Fix on Wheels, a mobile phone and laptop repair van in Ghent (Rune Waltniel & Lothar Van Cauwenbergh).

Everything is in one file: `index.html`. Open it in a browser, no build step.

## Before going live

At the top of the `<script>` in `index.html`, edit `CONFIG`:

- `bookingEmail` – where booking requests are sent (the form opens the visitor's email app)
- `tiktok`, `instagram` – your profile links

The prices in `index.html` are placeholders: check every one before you rely on them. Each phone in `PRICES` has a screen price, a battery price and a tier (1 to 4); the tier sets the price of all other repairs through `PHONE_REPAIRS`. Laptop extras are in `LAPTOP_REPAIRS`. Prices live in the `PRICES` object and time slots in `WEEKDAY_SLOTS` / `SAT_SLOTS`. The "taken" slots are simulated; connect a real booking tool (Calendly, Cal.com, a form backend) when you're ready.

## Host it free

GitHub: Settings → Pages → Deploy from branch `main`, folder `/ (root)`.
