# GHG Inventory Excel Model

A formula-driven Scope 1–3 GHG inventory workbook in Excel — the same tab structure and discipline (activity data, a cited emission-factor library, formula-linked totals, zero hardcoded results) used in a real client-facing carbon accounting engagement.

![Preview](preview.png)

**[Download the workbook →](GHG_Inventory_Excel_Model.xlsx)**

## Why I built this

Carbon accounting delivery runs heavily on Excel — client inventories, factor libraries and disclosure summaries all live there. This model proves I can build that structure correctly: every number is a formula, nothing is pasted in as a static value, and the whole thing recalculates when inputs change.

## What's inside

Three tabs, fully linked:

- **Activity Data** — one row per activity (year, site, scope, activity type, quantity), for a fictional two-site company (FY2025–FY2026). Emissions are calculated with `INDEX`/`MATCH` against the factor library — edit a quantity here and everything downstream updates.
- **Emission Factors** — a cited factor library (kgCO2e per unit), sourced from published UK DEFRA GHG Conversion Factors and US EPA datasets, with the exact source named per line.
- **Scope Summary** — `SUMIFS`-driven Scope 1/2/3 totals by year, a year-on-year chart, and a simplified **CDP Climate Change-style disclosure summary** (C6.1 / C6.3 / C6.5 / C6.10) mapped off the same formulas.

## Data quality

Recalculated and verified with zero formula errors. Colour-coded per standard financial-modelling convention: blue = hardcoded input, black = formula, green = cross-sheet link, yellow fill = key assumption/input cell.

## Methodology

Built to the **GHG Protocol Corporate Accounting and Reporting Standard** and the **GHG Protocol Scope 2 Guidance**. Emission factors are illustrative — compiled from published UK DEFRA and US EPA datasets for demonstration, not for actual client or regulatory reporting without independent verification.

## Disclaimer

Self-directed portfolio project, not audited. Not for regulatory disclosure or client use without independently verifying every factor and assumption.

## Author

**Rahul Christhuraj Latharani** — [Portfolio](https://rahulchris765-creator.github.io/) · [LinkedIn](https://linkedin.com/in/rahul-christhuraj)
