# STEPS-INDIA CRCT Sample Size Calculator

Interactive web tool for finalizing cluster count and sample size for the STEPS-INDIA cluster randomized controlled trial (CRCT) of the Enhanced Community Engagement Strategy (eCES).

## Features

- **Pre-populated with baseline survey data** (April 2026, N=4695, 237 clusters, 6 sites)
- **Co-primary outcomes**: BP control (hypertension) and glycemic control (diabetes)
- **Site-wise ICCs** from GEE with exchangeable correlation, with pooled substitution where ICC=0 or data insufficient
- **Dual powering**: study-level vs site-level independent powering
- **Sensitivity analysis**: interactive charts for ICC, cluster size, and minimum detectable effect
- **Export Summary**: downloadable HTML report for meeting minutes
- **Protocol V3 comparison**: side-by-side with original protocol assumptions

## ICC Methodology

ICCs estimated using two methods from the baseline cross-sectional survey:
- **ANOVA** (Donner 1986; Ridout et al. 1999)
- **GEE** with exchangeable correlation (preferred for binary outcomes)

Sites with ICC=0 or insufficient data (<200 participants) use the overall pooled GEE estimate.

## Key Findings (April 2026 Survey)

| Parameter | Survey (GEE) | Protocol V3 |
|-----------|-------------|-------------|
| ICC (BP control) | 0.0386 | 0.10 |
| ICC (glycemic control) | 0.0632 | 0.05 |
| Baseline BP control rate | 19.8% | 22.0% |
| Baseline glycemic control rate | 32.0% | 30.0% |

## Deployment

Deployed automatically via GitHub Pages on push to `main`.

## References

- Donner & Klar (1981); Hayes & Bennett (1999)
- Eldridge, Ashby & Kerry (2006); Rutterford, Copas & Eldridge (2015)
- Zou & Donner (2004); van Breukelen & Candel (2012)

---
STEPS-INDIA | ICMR-NHRP Funded | Investigators' Meeting, Jammu, April 2026
