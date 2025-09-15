# Detecting Publication Bias in Meta-Analysis

This project investigates statistical methods for detecting and addressing **publication bias** in meta-analysis.  
It illustrates applied statistical computing in R, combining methodological rigor with reproducible workflows.

---

## Objectives
- Explore methods to identify bias in published research
- Apply regression-based tests (e.g., Egger’s regression)
- Model selection mechanisms that drive bias
- Demonstrate corrections using state-of-the-art R packages
- Communicate findings with reproducible reports

---

## Methods and Tools
- **R Programming** for statistical analysis and reproducibility
- **RMarkdown/Quarto** for integrated code and narrative reporting
- **Core Packages:**
  - `metafor`: effect size computation, random- and mixed-effects models
  - `clubSandwich`: robust variance estimation
  - `weightr` / `selection.model`: publication bias modeling
  - `ggplot2`: funnel plots, forest plots, and diagnostics

---

## Example Analyses
- Funnel plots to visualize asymmetry  
- Egger’s regression test for small-study effects  
- Selection models for adjusting bias  
- Robust variance estimation for sensitivity analysis  

---

## Reproducibility
The analysis is contained in RMarkdown, ensuring that results are **transparent and reproducible**.  
To reproduce:
```r
# Install required packages
install.packages(c("metafor", "clubSandwich", "ggplot2"))
# For bias modeling
install.packages("weightr")

# Render the report
rmarkdown::render("Detecting-PB.Rmd")
