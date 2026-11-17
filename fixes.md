# Broken / fixed notes – E2

## 1. Contact form JavaScript file name

**Problem:** `contact.html` loaded `script.js`, but the repository contained the same script under the name `script (1).js`. A browser looking for `script.js` could not load the validation code.

**Fix:** The file is now named `script.js`, matching the path in the HTML. The old confusingly named duplicate was removed.

**How to check:** Open `contact.html`, open Developer Tools → Network, reload the page and check that `script.js` loads successfully. Then try an invalid registration number and a date in the past.

## 2. Missing shared site styling

**Problem:** The four HTML pages did not link to a shared stylesheet, so they had no consistent E2 visual design or responsive layout.

**Fix:** Added one `style.css` file and linked it from `index.html`, `about.html`, `listing.html` and `contact.html`. It contains the colour, font, spacing, Flexbox, Grid, responsive, dark-mode, focus, reduced-motion and print rules.

**How to check:** Open each page and confirm that the same header, navigation, typography and footer styling appear. In the Network panel, confirm that `style.css` loads with status 200 on all four pages.

## 3. Responsive and accessibility checks

**Existing item kept:** All four pages already had a viewport meta tag. Those tags were kept so mobile browsers use the device width.

**Fix:** The stylesheet uses a mobile-first layout, wrapping navigation, fluid headings, flexible service cards, visible keyboard focus and system colour preferences. No inline styles or CSS frameworks were added.

**How to check:** Test at 320 px, 360 px, 768 px and 1280 px. At 320 px, there should be no sideways scrolling. Use Tab to move through links and form controls, and test both light and dark system themes.
