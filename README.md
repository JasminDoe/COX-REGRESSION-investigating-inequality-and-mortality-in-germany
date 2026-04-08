# Socioeconomic Inequality and Mortality in Germany

## Overview
This project examines the association between socioeconomic status and mortality risk in Germany using survival analysis.

Socioeconomic status is approximated using burial type, comparing urn burials (lower cost) to traditional grave burials (higher cost). Age at death is derived from birth and death dates. Sex is included as a covariate.

---

## Research Question
How is socioeconomic status, proxied by burial type (urn vs. grave), associated with mortality risk?

---

## Data
- `cemetery_clean.csv`: dataset containing individual-level information on birth date, death date, sex, and burial type  
- Time-to-event variable constructed from lifespan (age at death)  

---

## Methods
- Cox proportional hazards models  
- Outcome: time to death (age at death)  
- Exposure: burial type (urn vs. grave)  
- Covariate: sex  
- Implemented in R (`survival`, `tidyverse`)  

---

## Files
- `Analysis.qmd`: reproducible analysis document  
- `rstudio_analysis.R`: main R script  
- `Analysis.html`: rendered report  
- `Socioeconomics and Survival_short.pptx`: presentation slides  

---

## Reproducibility
1. Open `Analysis.qmd` or `rstudio_analysis.R` in RStudio  
2. Run the script or render the Quarto document  
3. Results correspond to the provided HTML output  

---

## Key Findings
- Burial type is associated with differences in mortality risk  
- Contrary to expectations, urn burials are associated with lower hazard rates than grave burials  

---

## Interpretation and Limitations
- Burial type may not be a valid proxy for socioeconomic status  
- The observed association likely reflects unmeasured factors, such as cultural preferences or personality traits  
- Results should be interpreted cautiously due to potential confounding and proxy misclassification  

