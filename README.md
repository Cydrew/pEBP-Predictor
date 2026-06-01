# pEBP Advisor

A patient-conditional decision-support tool for **prophylactic epidural blood patch (pEBP)** following recognised accidental dural puncture (ADP) with a Tuohy needle during attempted labour epidural placement.

## What it does

The tool renders published evidence (meta-analyses, RCTs, prospective cohorts) as a per-patient computation. Given patient characteristics — age, BMI, hours since ADP, Tuohy gauge, risk and protective modifiers, contraindications — it produces:

- A predicted PDPH probability (conditional on ADP having occurred)
- An estimated number-needed-to-treat
- A position on a benefit-versus-harm decision chart
- A transparent, scrutable breakdown of every coefficient used

## Scope

This tool addresses **one** clinical decision: whether to administer prophylactic epidural blood patch through an in-situ epidural catheter after a recognised wet tap with a Tuohy needle during attempted labour epidural placement.

It does **not** apply to:
- Post-spinal (intentional dural puncture) headache
- Diagnostic lumbar puncture
- Combined spinal-epidural or dural-puncture-epidural techniques without Tuohy ADP

## Important notes

- **Not a meta-analysis.** Published meta-analyses are its inputs; it renders them per-patient.
- **Not validated against patient outcomes.** Coefficients are anchored to literature point estimates from cohorts that may not match your institution. Treat outputs as evidence-informed estimation, not calibrated risk prediction.
- **Not a guideline.** It helps interpret existing guidelines (Uppal 2023 multisociety consensus; SOAP; ASRA) against an individual patient.
- **Not AI.** No machine-learning model. All coefficients and equations are exposed and stable. Parameters that are model-derived rather than literature-extracted are marked with a dagger (†).

## Evidence anchoring

Base rate (55% for 17G Tuohy ADP) is anchored to Maranhao 2021 network meta-analysis, Choi 2003 systematic review (52.1% pooled), and Heesen 2019 systematic review. Efficacy anchored to Stein 2014 RCT. Full sourcing, including the distinction between literature-derived and model-derived parameters, is documented in the tool's "Methods & scoring" tab.

## Running it

This is a single self-contained HTML file. No server, no build step, no dependencies beyond a CDN-loaded charting library. Open `index.html` in any modern browser, or visit the hosted version.

## Version

v1.1 — evidence reviewed 2026.

## License

Icahn School of Medicine at Mount Sinai. 

## Disclaimer

For clinical decision support and educational use only. Does not replace clinical judgement, institutional protocols, or informed consent.
