# CGAF 9(a) – Quick PDF Filler (Cebu BI)

This is a static web page that fills the official **Bureau of Immigration (Philippines)** CGAF form (Rev. Lev. 4, Effective 07 AUG 2024) with constant data, and lets you choose **Date of Latest Arrival** and **Months to Extend** (1 / 2 / 6). It downloads a print‑ready PDF that you can sign and submit at Robinsons Galleria Cebu (BI).

> The base form is provided by BI and marked: *"This document may be reproduced and is NOT for sale."*

## How to deploy to GitHub Pages

1. Create or use an existing repository (already created: `Form9A`).
2. Put three files in the repo root:
   - `index.html`  ← the web app
   - `form.pdf`    ← the official CGAF form (this repo includes it)
   - `README.md`
3. Commit & push to `main`.
4. In **Settings → Pages**:
   - **Source**: `Deploy from a branch`
   - **Branch**: `main` (root)
   - Save. Wait for the green check.

Your site will be served at `https://<your-username>.github.io/Form9A`.

## Usage
- Open the site on your phone.
- Select **Date of Latest Arrival**; months default to **One (1) month**.
- (Optional) Enter Flight No. or leave blank.
- Click **Generate PDF** → a file like `KEI_NISHIKAWA_CGAF_2025-10-06_M1.pdf` downloads.
- Print A4 (B/W ok) at the mall; sign at BI counter.

### Fine‑tuning
If your printer adds margins that cause tiny misalignment, adjust **Nudge X/Y** (points). Re‑generate and print again.

## Notes
- All constant personal details are hard‑coded in `index.html` under `CONST`.
- To change default months, edit the `<select>` element or code.
- 
