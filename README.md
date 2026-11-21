# dri-milk-report

Bilingual DRI milk tools for WhatsApp sharing:

1. **Centre Report** (`index.html`) — daily milk collection centre report (cow/buffalo fat, LR, SNF, quantity, van timings).
2. **Income Calculator** (`income-calculator.html`) — individual farmer milk income from analyzer Fat, LR and temperature using the **JSDS rate revision effective 21.11.2026**.

## Income calculator

Enter Fat (%), Lactometer Reading (LR), milk temperature (°C) and quantity (L). The tool:

- Corrects LR → CLR using the JSDS temperature table
- Looks up ₹/litre from the Fat × CLR (25–30) chart
- Shows estimated income and can preview / copy / send on WhatsApp

Rates: cow milk up to 5.5% fat at ₹308/kg total solids; buffalo from 5.6% fat at ₹850/kg fat (as published by Jabalpur Sahakari Dugdh Sangh Maryadit).

Open either HTML file in a browser — no build step required.
