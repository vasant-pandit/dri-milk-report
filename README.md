# dri-milk-report

Bilingual DRI milk tools for WhatsApp sharing:

1. **Centre Report** (`index.html`) — daily milk collection centre report (cow/buffalo fat, LR, SNF, quantity, van timings).
2. **Income Calculator** (`income-calculator.html`) — individual farmer milk income from analyzer Fat, LR and temperature using the **JSDS rate revision effective 21.11.2026**.

## Income calculator

Select milk type (cow/buffalo), then enter Fat (%), Lactometer Reading (LR 25–30) and quantity (L). The tool:

- Looks up ₹/litre from the Fat × LR (25–30) chart
- Shows estimated income and can preview / copy / send on WhatsApp

Rates: cow milk up to 5.5% fat at ₹308/kg total solids; buffalo from 5.6% fat at ₹850/kg fat (as published by Jabalpur Sahakari Dugdh Sangh Maryadit).

Open either HTML file in a browser — no build step required.

## Deploy on Render (public URL)

This repo includes a Render Blueprint (`render.yaml`) for a free static site.

1. Open **[Deploy to Render](https://render.com/deploy?repo=https://github.com/vasant-pandit/dri-milk-report)**  
   (or in the [Render Dashboard](https://dashboard.render.com/): **New → Blueprint** / **New → Static Site**, connect `vasant-pandit/dri-milk-report`).
2. Select branch `cursor/jsds-milk-income-calculator-f53f` (or `main` after the PR is merged).
3. **Build Command:** leave as `true` (no build).
4. **Publish Directory:** `.`
5. Click **Create Static Site** / **Apply**.

After deploy, your public URLs will look like:

- Centre report: `https://<your-service>.onrender.com/`
- Income calculator: `https://<your-service>.onrender.com/income-calculator.html`  
  (also `/calculator` and `/income`)
