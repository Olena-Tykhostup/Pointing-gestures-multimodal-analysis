This folder contains the R scripts and data for one of the chapters of the dissertation titled 

"Multimodal Annotation and Analysis of a Narrative Problem-Solving Task in English, Idi, and Russian"

by 

Olena Tykhostup

Specifically, this part of the project deals with the analysis reported in Chapter 6, focusing on the effect of common ground on pointing gestures.

The project directory is structured as follows:

scripts/: Contains R scripts and packages used for the analysis.

- 01-Pointing_gestures_and_common_ground_duration.Rmd:  Analyzes the relationship between pointing gestures durations and information status of co-produced spoken epxressions in English, Russian, and Idi.
 
- 02-Pointing_gestures_and_common_ground_logistic_regression.Rmd: Analyzes the relationship between different form-realted variables in pointing gestures (hand shape, contact with the target, etc) and the information status of co-produced spoken epxressions in English, Russian, and Idi by the means of a series of logistic regression models.

data/: Contains the datasets used in the analyses.
figures/: Stores the generated figures from the analysis scripts.

Some R packages are required to run the scripts. You can install these packages using the following commands in R:

install.packages(c(
  "here",         # File paths relative to the top-level directory
  "lubridate",    # Dates and times
  "ggplot2",      # Visualisations 
  "tidyverse",    
  "sjPlot",       # Data visualization
  "lme4",         # Linear mixed-effects models 
  "ggeffects",    # Marginal effects for 'ggplot' from model outputs
  "gtable",       # Arrange 'grobs' in tables
  "performance",  # Assessment of regression models performance
  "car",          # Companion to Applied Regression
  "ggbeeswarm",   # Column scatter / beeswarm-style plots
  "ggpubr"        # 'ggplot2' Based Publication Ready Plots
))
