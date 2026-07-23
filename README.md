
## Version History

### v2.0 (Current — Recommended)

- Corrected risk contribution analysis using **standardized regression coefficients**
- Enhanced **Figure 4 (CDF)** with improved visibility and annotations
- Added **CAPEX/OPEX** distinction in cost classification
- Corrected **probability of cost overrun** with meaningful thresholds
- Updated **VaR and CVaR** calculations with overrun percentages
- Improved **Sankey diagram** with corrected flow widths

### v1.0 (Original)

- Initial implementation of Chang & Ko (2017) methodology
- Basic Monte Carlo simulation with 10,000 iterations
- Standard risk metrics (VaR, CVaR)
- Preliminary figures and visualizations

## Features

- **Lognormal Parameter Estimation:** Automatic estimation of μ and σ from three-point estimates (minimum, mode, maximum)
- **Correlated Monte Carlo Simulation:** 10,000 iterations using Cholesky decomposition
- **Risk Metrics:** Value at Risk (VaR), Conditional VaR (CVaR), probability of cost overrun
- **Sensitivity Analysis:** Standardized regression coefficients and variance decomposition
- **Scenario Analysis:** Optimistic, Most Likely, and Pessimistic scenarios
- **Publication-Ready Figures:** Histograms, CDF, boxplots, pie charts, Sankey diagram

## Key Results (v2.0)

| **Metric** | **Value** |
|------------|-----------|
| Mean Total Cost | $538.3M |
| Standard Deviation | $48.9M |
| P(Cost > Baseline) | 46.07% |
| P(Cost > 20% Overrun) | 1.51% |
| VaR (95%) | $621.8M (14.7% overrun) |
| CVaR (95%) | $645.8M (19.2% overrun) |

**Risk Contributions (Standardized Regression):**

| **Component** | **Contribution** |
|---------------|------------------|
| Operational Costs | 53.84% |
| Electrical Infrastructure | 20.28% |
| PSA Oxygen Plant | 13.47% |
| Surgical Bed Expansion | 12.41% |

## Data Sources

Cost estimates were derived from:

- Project documentation (Rönesans Holding, 2023)
- Industry benchmarks (FreshBooks, 2024; Sdino & Rosasco, 2024)
- Peer-reviewed literature (Vieira et al., 2022; Halil et al., 2024)

## System Requirements

| **Requirement** | **Version** |
|-----------------|-------------|
| Python | 3.10+ |
| NumPy | 2.0.0+ |
| Pandas | 2.2.0+ |
| Matplotlib | 3.8.0+ |
| Seaborn | 0.13.0+ |
| SciPy | 1.13.0+ |
| Scikit-learn | 1.5.0+ |
| Plotly | 5.0.0+ |

## Installation and Usage

### 1. Clone the Repository

```bash
git clone https://github.com/[YourUsername]/adana-hospital-monte-carlo.git
cd adana-hospital-monte-carlo
