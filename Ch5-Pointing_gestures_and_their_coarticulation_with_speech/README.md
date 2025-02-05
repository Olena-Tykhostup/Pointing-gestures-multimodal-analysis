This folder contains the R scripts and data for one of the chapters of the dissertation titled 

"Multimodal Annotation and Analysis of a Narrative Problem-Solving Task in English, Idi, and Russian"

by 

Olena Tykhostup

Specifically, this part of the project deals with the analysis reported in Chapter 5, focusing on the relationships between pointing gestures and spoken expressions. It investigates the temporal, semantic, and structural relationships between spoken expressions in English and Russian and the co-produced pointing gestures.

The project directory is structured as follows:

scripts/: Contains R scripts and packages used for the analysis.

- 01-Temporal-Coordination.Rmd: Analyzes the timing and temporal coordination between pointing gestures and speech in English.

- 02-Collostructional-Analysis.Rmd: R script for collostructional analysis in English and Russian.

- 03-Pointing-forms-variation.Rmd: Examines the variations in pointing gesture forms in English and Russian.

- collostructions_0.2.0.tar.gz: The R package for collostructional analysis. Flach, Susanne. 2021. Collostructions: An R implementation for the family of collostructional methods. Package version v.0.2.0, https://sfla.ch/collostructions/.

- UDpipe models for tokenizing and part-of-speech tagging: russian-gsd-ud-2.5-191206.udpipe, english-ewt-ud-2.5-191206.udpipe. Wijffels, Jan. 2021. Udpipe: Tokenization, Parts of Speech Tagging, Lemmatization and Dependency Parsing with the ’UDPipe’ ’NLP’ Toolkit. https://CRAN.R-project.org/package=udpipe.

data/: Contains the datasets used in the analyses.
figures/: Stores the generated figures from the analysis scripts.

Some R packages are required to run the scripts. You can install these packages using the following commands in R:

install.packages(c(
  "here",          # Create paths relative to the top-level directory
  "tidyverse",     # A collection of R packages designed for data science
  "lubridate",     # Work with dates and times
  "readtext",      # Reading text data
  "hunspell",      # Spell check and stemming
  "udpipe",        # Tokenization, part of speech tagging, lemmatization and dependency parsing with the UDPipe natural language processing toolkit
  "dplyr",         # A grammar of data manipulation
  "tidyr",         # Easily tidy data with spread and gather functions
  "stringr",       # Wrappers for common string operations
  "FactoMineR",    # Multivariate exploratory data analysis and data mining
  "factoextra",    # Extract and visualize the results of multivariate data analyses
  "patchwork",     # The Composer of Plots
  "ggforce"        # Accelerating ggplot2
))

# For the collostructions package, you can to install it from a local source
install.packages(here("scripts", "collostructions_0.2.0.tar.gz"), repos = NULL, type = "source")
