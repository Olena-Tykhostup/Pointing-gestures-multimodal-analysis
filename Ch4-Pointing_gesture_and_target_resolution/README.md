This folder contains the R scripts and data for one of the chapters of the dissertation titled 

"Multimodal Annotation and Analysis of a Narrative Problem-Solving Task in English, Idi, and Russian"

by 

Olena Tykhostup

Specifically, this part of the project deals with the analysis reported in Chapter 4, focusing on the agreement between three annotators regarding the targets of pointing gestures under different conditions and the analysis of pointing gesture form-related variables and pointing gesture targets annotated in the annotation condition when the annotators had no access to the spoken channel of communication.

The project directory is structured as follows:

scripts/: Contains two R scripts used for the analysis.

- 01-Agreement-Target-Resolution.Rmd: Analyzes and visualizes the agreement between three annotators on the targets of pointing gestures under three annotation conditions: Gesture, card, speech; Gesture and card; Gesture only.

- 02-Target-Resolution-No-Speech.Rmd: Generates mosaic plots to visualize frequencies of occurrence of form-related variables (hand shape, hand orientation, trajectory of movement, contact with the target) and target types (individual item within a card, a section within a card, everything/anything in the card). Conducts chi-squared tests and fits a conditional inference tree. Develops a Conditional Random Forest model and evaluates it with Partial Dependence Plots and visualization of predicted probabilities.

data/: Contains the datasets used in the analyses.
figures/: Stores the generated figures from the analysis scripts.

Some R packages are required to run the scripts. These packages can be installeld using the following commands in R:

install.packages(c(
  "here",          # Easy paths relative to the project root
  "tidyverse",     # Collection of data science packages
  "DescTools",     # Kappa values Confidence Intervals
  "irr",           # Kappa values calculation
  "ggmosaic",      # For creating mosaic plots
  "patchwork",     # Combining multiple ggplot2 plots into one
  "party",         # Recursive partitioning for classification, regression, and survival trees
  "partykit",      # A toolkit for recursive partytioning
  "ggparty",       # Visualizing decision trees from party with ggplot2
  "caret",         # Classification and regression training
  "pdp",           # Partial dependence plots
  "scales"         # Scale functions for visualization
))

