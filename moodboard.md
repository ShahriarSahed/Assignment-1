# Mood board: Autokorjaamo Hakola

## Feeling

**Trustworthy, practical and welcoming.**

- **Trustworthy:** A deep navy header and footer, clear typography and readable contrast make the workshop feel established and dependable.
- **Practical:** A straightforward page structure, service cards and a clearly visible service-request action help visitors find what they need without learning technical terms.
- **Welcoming:** A warm off-white background softens the darker workshop colours. The writing stays direct and friendly.

The design is for a small, family-run repair shop in Kauhava that works with cars, vans and farm vehicles. The customer brief does not provide a logo, photographs or brand colours, so this concept uses a simple colour system rather than pretending that the workshop has supplied brand assets.

## Colours

| Name | Hex | Used for |
|---|---|---|
| Warm canvas | `#F5F2EB` | Main light-mode background |
| White | `#FFFFFF` | Content cards and form fields |
| Charcoal | `#202A35` | Main text |
| Slate | `#4B5967` | Secondary text |
| Workshop brown | `#7A3518` | Links and main action in light mode |
| Deep navy | `#1C2E3A` | Header and footer |
| Workshop amber | `#F2B544` | Active navigation and keyboard focus on dark header |
| Night background | `#111A22` | Dark-mode background |
| Night surface | `#1A2732` | Dark-mode cards |
| Light text | `#F4F1EA` | Main dark-mode text |
| Light slate | `#BBC6CE` | Secondary dark-mode text |
| Warm orange | `#F1A35B` | Dark-mode links and main action |

### Text contrast checks

The following foreground/background pairs were checked using the WCAG contrast-ratio calculation. Normal text needs at least 4.5:1.

| Text use | Foreground | Background | Ratio |
|---|---|---|---:|
| Main light-mode text | `#202A35` | `#F5F2EB` | 13.01:1 |
| Secondary light-mode text | `#4B5967` | `#F5F2EB` | 6.42:1 |
| Light-mode links | `#7A3518` | `#F5F2EB` | 7.99:1 |
| Light button text | `#FFFFFF` | `#7A3518` | 8.94:1 |
| Main dark-mode text | `#F4F1EA` | `#111A22` | 15.58:1 |
| Secondary dark-mode text | `#BBC6CE` | `#1A2732` | 8.75:1 |
| Dark-mode links | `#F1A35B` | `#111A22` | 8.48:1 |
| Dark button text | `#17212B` | `#F1A35B` | 7.86:1 |
| Active navigation/focus | `#F2B544` | `#1C2E3A` | 7.64:1 |

The page changes its colour tokens with `prefers-color-scheme`, so the same components work in light and dark modes. The focus indicator also changes to stay visible on the dark header.

## Fonts

Use the device's system sans-serif font stack. It is familiar, readable and does not require an external font download. Headings use the same family with a heavier weight, so the site stays visually consistent and loads without a third-party font request.

## Layout

- The header places the workshop name before a wrapping navigation row on small screens. On wider screens, Flexbox puts the name on the left and navigation on the right.
- The page uses a single-column mobile-first layout. At `48rem`, the services page uses a Grid layout with auto-fitting columns.
- Service sections are cards with consistent spacing and borders. The layout uses the content's available width rather than fixed device sizes.
- The footer is kept at the bottom on short pages with a three-row body grid.
- Form controls are full-width and large enough to use with a finger.
- Images are constrained to their container. Long words can wrap rather than forcing horizontal scrolling.
- Reduced-motion, higher-contrast and print preferences have dedicated media queries.

## References

The three workshop websites reviewed for the project are documented in [plan.md](plan.md): [CarOn](https://caron.fi/en/), [InCar](https://www.incar.fi/en/) and [ALL Motors](https://allmotors.fi/en/services). They are references for service information and navigation ideas, not designs or text to copy.

## Assets still needed from the customer

Ask Autokorjaamo Hakola for its approved logo, workshop photographs, exact contact details and opening hours before treating this concept as the final business identity. These details were not included in the customer brief and have not been invented.
