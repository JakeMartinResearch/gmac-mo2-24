# 🐟 gmac-mo2-24: Oxygen Consumption and Hypoxia Tolerance in *Galaxias maculatus*

This repository contains R code and data used to analyse metabolic responses to salinity and hypoxia in the Common Galaxias (*Galaxias maculatus*), with a focus on estimating critical oxygen thresholds (Pcrit) and understanding patterns of oxyregulation.

---

## 📄 Project Summary

- **Title**: The role of osmorespiratory compromise in hypoxia tolerance of the purportedly oxyconforming teleost *Galaxias maculatus*

- **Authors**: Timothy D. Clark ^[a]^, Luis L. Kuchenmüller ^[a]^, Elizabeth C. Hoots ^[a]^, Maryane Gradito ^[a]^, and Jake M. Martin ^[a,b]^ 

- **Institutions**: [a] School of Life and Environmental Sciences, Deakin University, Geelong, VIC, Australia, and [b] School of Biological Sciences, Monash University, Clayton, VIC, Australia 

- **Status**: 🚧 Unpublished and ongoing 🚧 

With *G. maculatus* as a model, we test (1) whether this species exhibits oxyregulation, and (2), whether isosmotic conditions can ease the osmorespiratory compromise to reduce resting oxygen uptake rates and improve hypoxia tolerance. This project compares the standard metabolic rate (SMR), routine metabolic rate (RMR), and estimates Pcrit values across fish exposed to different salinity treatments, freshwater (0  ppt) or isosmotic conditions (9  ppt). Data were collected using intermittent-flow respirometry and analysed in R (v4.2.3).

An HTML version of the R script is available here:  
📍 [https://jakemartinresearch.github.io/gmac-mo2-24/](https://jakemartinresearch.github.io/gmac-mo2-24/)

---

## 📁 Repository Structure

```
📆 gmac-mo2-24/
🗄️ input-data/           # Raw and cleaned input data
🗄️ mod-data/             # Intermediate data and summaries for modelling
🗄️ output-fig/           # Final figures used in the manuscript
🗄️ output-mod/           # Model outputs (e.g. .rds files)
🗄️ gmac-labchart-24.Rmd  # Main analysis and figure generation script
🗄️ index.html            # Rendered HTML results file
🗄️ EXP-2024-gmac-labchart.Rproj  # RStudio project file
```

---

## 📦 R Dependencies

This project uses the following key packages:

Data Visualisation
-`ggthemes` 
-`bayesplot`
-`gt`
-`gtsummary`
-`plotly` 
-`qqplotr`
  
Tidy Data and Wrangling
-tidyverse
-janitor
-readxl
-broom.mixed
-data.table
-hms
-devtools
-mclust
  
Modelling and Statistical Analysis
-brms 
-rstan 
-marginaleffects 
-performance 
-emmeans
-tidybayes 
-respirometry 
-future   

In the R markdown docment you will install/load these using `p_load` from in `pacman`

---

## 🔍 Key Methods

- **SMR estimation**: Custom implementation of Chabot et al.'s `calcSMR` method

- **Incremental regression**: Bayesian polynomial regression to model MO₂–DO relationships (Urbina et al., 2012)

- **Pcrit detection**: Rule-based method following Claireaux & Chabot (2016), with visual validation

- **Model comparison**: Performed using leave-one-out cross-validation (LOO-CV)

---

## 📊 Outputs

- Figures and summary statistics are rendered into a browsable HTML site:  
  📍 [https://jakemartinresearch.github.io/gmac-mo2-24/](https://jakemartinresearch.github.io/gmac-mo2-24/)
  
- Each model’s diagnostic and output values are saved in `.rds` files for reproducibility.

---

## 📥 Download or Pull This Repository into R

To work with this project in R, you can clone or download it directly from GitHub using RStudio.  

Open RStudio: Click File → New Project → Version Control → Git.

In the Repository URL box, paste:

```
https://github.com/JakeMartinResearch/gmac-mo2-24.git
```

Choose a folder on your computer to save the project.   

Click Create Project — RStudio will pull the project into a new folder and open it automatically.   

📺 Tutorial: How to clone a GitHub repo into RStudio (YouTube, 2 min)  

---

## 📘 Citation

🚧 To be added 🚧

---

## 📩 Contact

Jake M. Martin  
Email: [jake.martin1@monash.edu](mailto:jake.martin1@monash.edu)  
ORCID: [https://orcid.org/0000-0002-XXXX-XXXX](https://orcid.org/)

---
