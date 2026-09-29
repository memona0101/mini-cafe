# Ember & Oak — Coffee Roasters

A one-page website for Ember & Oak, a small-batch roastery and café on Kiln Street.
It's a single HTML file with no build step or dependencies. Open it in a browser and it runs.

## Features

- **Daily roast ticket:** a printed-style ticket in the hero that changes every day. It cycles through 11 origins and shows the batch number, process, first crack, drop temperature and tasting notes.
- **Interactive roast curve:** drag along the curve (or tap a stage) to follow a 10-minute roast from charge to drop. The temperature and timer update live.
- **Menu:** a printed-menu layout with dotted leaders to the prices, plus a "Today's pour-over" card that matches the daily roast ticket.
- **Gallery:** a film-style contact sheet of 14 photos with category filters (Bar, Roastery, Room, Kitchen) and a full-screen viewer. The viewer supports keyboard arrows, swipe and Esc.
- **Live opening status:** a clock and an open/closed badge worked out from the posted hours, with today's row highlighted in the hours table.
- **Navigation:** smooth scrolling to each section, highlighting of the current section, and a menu for phones.
- **Contact:** tap-to-call on phones. On desktop, "Call ahead" shows the number and copies it. Also includes email and map directions links.
- **Responsive and accessible:** works on phone and desktop, supports keyboard navigation, and respects the "reduced motion" setting.

## Run it locally

Open `ember-and-oak-cafe.html` in any modern browser. That's it.

To serve it locally instead (optional):

```bash
npx serve .
```

## Built with

- Plain HTML, CSS and JavaScript (no frameworks)
- Google Fonts: Fraunces, Newsreader, Courier Prime, Reenie Beanie
- Photos from [Unsplash](https://unsplash.com)

## Customizing

Everything lives in `ember-and-oak-cafe.html`:

| What | Where to look |
|---|---|
| Colors | the `:root` variables at the top of the `<style>` block |
| Daily origins and tasting notes | the `ORIGINS` array in the `<script>` |
| Roast curve stages | the `STAGES` array in the `<script>` |
| Gallery photos and captions | the `PHOTOS` array in the `<script>` (Unsplash photo IDs) |
| Opening hours | the hours table in the Visit section, and the `tick()` function |
| Menu items and prices | the Menu section in the HTML |

## Before going live

- Replace the placeholder address, phone number and email. The address `412 Kiln Street` is fictional, so the directions link won't find a real place until it's updated.
- Swap the Unsplash photos for your own, or download them and host them with the site.
- Update the roaster's signature, the house rules and the origin list to match the real café.

## License

© 2026 Ember & Oak Coffee Roasters. All rights reserved.
