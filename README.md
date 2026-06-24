# Corporate Tax Estimation & Penalty Calculator

A single-file web tool for Malaysian tax consultants to estimate corporate tax,
identify the Section 107C(10) under-estimation penalty, and plan how much taxable
income to reduce in order to stay within the safe zone.

## Usage

Open `index.html` in any modern browser — no build step or server required.
(Built with React + Tailwind CSS loaded from CDNs.)

## Features

- **SME / Non-SME toggle** — SME progressive rates (15% / 17% / 24%) or a flat 24%.
- **Direct tax inputs** — enter Estimated Tax Payable (ET) and Actual Tax Payable (AT).
- **Implied taxable income** — back-calculated from each tax figure using the active rate rules.
- **Penalty computation** — `[ (AT − ET) − (30% × AT) ] × 10%`, with the 10% penalty highlighted in red.
- **Maximum taxable income without penalty** — the income whose tax equals the safe ceiling (ET ÷ 0.7).
- **Taxable income to reduce to avoid penalty** — implied actual income minus the max income without penalty.
- **Tier breakdown tables** showing how the tax maps across the SME bands.
- **Save as PDF** — exports a clean copy via the browser's print dialog.

> For internal advisory use. Verify against the latest LHDN rates and rulings before filing.
