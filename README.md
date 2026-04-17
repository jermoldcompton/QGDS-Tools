# QGDS Tools

A collection of interactive tools used to build, audit, and validate the foundations and assets of the [Queensland Government Design System](https://www.designsystem.qld.gov.au/) (QGDS).

---

## Purpose

QGDS Tools supports the development of a research-led, evidence-based design system for the Queensland Government. Each tool in this repository addresses a specific aspect of design system foundations, from token scale architecture to spacing, sizing, and grid relationships, providing practitioners with a transparent, explorable reference for the decisions that underpin the system.

---

## Tools

### QGDS Scales

An interactive reference tool for exploring the mathematical relationships between the three core token scales in the Queensland Government Design System: Grid, Size, and Spacing.

These scales share a stepped exponential structure with calibrated divergence rates, each tuned to the perceptual demands of its role:

| Scale | Formula | Role |
|---|---|---|
| Grid | Sₙ = Sₙ₋₁ + a × b^⌊(n−1)/c⌋ where a=2, b=2, c=24 | Common denominator, the base rate underpinning spacing and sizing |
| Size | Sₙ = Sₙ₋₁ + a × b^⌊(n−1)/c⌋ where a=4, b=2, c=12 | UI element sizing, doubles twice as fast as Grid |
| Spacing | Sₙ = Sₙ₋₁ + a × b^⌊(n−1)/c⌋ where a=4, b=2, c=8 | Spatial hierarchy, doubles three times as fast as Grid |

**Features**

- Interactive scale explorer with editable variables (S, a, b, c) per scale
- Live chart visualisation of cumulative values and increment growth
- px and rem unit toggle
- Configurable step count and table height
- Per-column and full-table copy for use in external spreadsheets
- Chart export as PNG
- Scale visibility toggles per chart line
- Responsive layout for desktop and mobile

**Preview:** https://jermoldcompton.github.io/QGDS-Tools/QGDS-Scales.html?v=26041701

---

## About

These tools are built and maintained by **Jermold Compton**, Senior UI and UX Designer, Queensland Government, in support of the QGDS foundations workstream.

For enquiries about the Queensland Government Design System, contact the QGDS team at [qgdesignsystem@qld.gov.au](mailto:qgdesignsystem@qld.gov.au).
