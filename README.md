# Investment Tracker PWA

Version 1.0.0 — neon-themed installable Progressive Web App based on the uploaded `MF.html` Step-Up SIP Allocation Framework.

## Included
- Splash screen with version number.
- Dynamic monthly SIP allocation across the six funds and percentages in the source HTML (35/20/10/15/10/10).
- Editable fund allocation weights; allocation amounts are normalised if entered weights do not sum to 100%.
- Target corpus, starting monthly SIP, annual step-up, mid-tenure SIP change, tenure and assumed return controls.
- Year-by-year monthly-compounding projection and target-achievability indicator.
- Portfolio table for invested/current values, gain/loss, return percentage and current-vs-target allocation drift.
- Local browser storage and JSON import/export.
- Manifest, app icon and service worker for offline PWA support.

## Publish
Enable GitHub Pages for the repository's `main` branch, root folder. Open the Pages URL over HTTPS and use the browser's Install / Add to Home screen action.

## Projection model
Each month's estimated value is compounded at the effective monthly rate derived from the entered annual return, then the SIP for that month is added. Figures are estimates, not guarantees. This tool does not model taxes, fund expenses, exit loads or market volatility. The fund names and target percentages are carried over from the supplied source HTML; review fund suitability and current scheme details independently.
