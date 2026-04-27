# Philippine Volcanic Eruptions Analysis

> Exploratory analysis of the top 5 deadliest Philippine volcanic eruptions using R, examining the relationship between VEI and death toll.

**Author:** RenzWoo &nbsp;|&nbsp; **Date:** April 2025

![Infographic](Philippine volcanic eruptions.png)

---

## Objective

This project examines two key variables from historical Philippine eruption data: the **Volcanic Explosivity Index (VEI)** and **death toll**. VEI was chosen because it provides a standardized measure of eruption intensity, giving a clear picture of each event's physical scale. Deaths were chosen because they reflect the real human consequences of each eruption — bridging the gap between geological power and community vulnerability. Together, these two variables allow us to ask whether more explosive eruptions necessarily mean more lives lost.

---

## Key Findings

1. **VEI alone does not predict mortality.**
   The correlation between VEI and deaths is weak (r = 0.19), meaning explosiveness explains only ~3.6% of the variation in fatalities. Hibok-Hibok's VEI 3 eruption, for example, proved deadlier than some VEI 4 events due to toxic gas exposure.

2. **Secondary hazards and proximity drive casualties.**
   Lahars accounted for roughly 60% of Pinatubo's deaths. Taal (1911) affected an estimated 500,000 people within 15 km. Mayon (1814) struck at night, limiting evacuation. Eruption type, population density, and timing matter more than raw explosivity.

3. **Emergency response and public awareness are critical.**
   Modern PHIVOLCS monitoring has demonstrably reduced fatalities. Effective early warning and evacuation systems can keep casualties low regardless of a volcano's VEI — the 1991 Pinatubo response saved thousands despite being the 20th century's largest eruption.

> **Note:** With only 5 data points, statistical results here are illustrative rather than definitive. The patterns are a starting point for deeper analysis with a larger dataset.

---

## Dataset

| Source | Details |
|--------|---------|
| [Database of Volcanic Eruptions — Kaggle](https://www.kaggle.com/) | Primary dataset (`Volcano-Philippines.csv`) |
| [PHIVOLCS](https://www.phivolcs.dost.gov.ph/) | Philippine Institute of Volcanology and Seismology |
| [NGDC/NOAA](https://www.ngdc.noaa.gov/hazard/volcano.shtml) | National Geophysical Data Center volcanic hazard records |

---

## Tech Stack

- **Language:** R
- **Libraries:** `tidyverse`, `ggplot2`, `readr`, `dplyr`
- **Report format:** R Markdown → PDF

---

## How to Run

```bash
# 1. Clone the repository
git clone https://github.com/your-username/philippine-volcanic-eruptions-analysis.git
cd philippine-volcanic-eruptions-analysis
```

```r
# 2. Install required R packages (run once in R or RStudio)
install.packages(c("tidyverse", "readr", "dplyr"))
```

3. Open `notebooks/analysis.Rmd` in RStudio.
4. Click **Knit → Knit to PDF** to reproduce the full report.

Output will be saved to `outputs/report.pdf`.

