# Overview

We used the template file and folder structure for a data analysis project/paper done with R/Quarto/Github from Dr. Andres Handel. 

# Pre-requisites

This data analysis project used R, Quarto, Github and a reference manager that can handle bibtex. It is also assumed that you have a word processor installed (e.g. MS Word or [LibreOffice](https://www.libreoffice.org/)). You need that software stack to make use of this template.

# Project structure

* All data goes into the subfolders inside the `data` folder.
* All code goes into the `code` folder or subfolders.
* All results (figures, tables, computed values) go into `results` folder or subfolders.
* All products (manuscripts, supplement, presentation slides, web apps, etc.) go into `products` subfolders.
* The `renv` folder is automatically generated by the `renv` package, and is used to keep track of packages.
* See the various `README.md` files in those folders for some more information.


# How to reproduce the project
* Begin with the `processing-file.qmd` file in the code > processing-code folder to load the raw data from the `AIU All Women Dataset.csv` file in the data > raw-data folder and process it accordingly. This document will clean all variables for analysis and save them in the `processeddata.rds` file located in the data > processed-data folder. 

* Visit the `eda.qmd` file in the code > eda-code folder to create exploratory figures and plots using the processed data to model the outcome, predictor variables, and covariates. All exploratory figures are saved in the results > figures > exploratory-figures folder. 

* Proceed to the `statistical-analysis.qmd` file in the code > analysis-code folder to explore various models for the data and subsequent techniques for model testing and parameter tuning. A detailed explanation of why we chose the final model as the LASSO regression model can be found in this file. All figures are saved in the results > figures > final-figures folder. 

* Create the manuscript in the products > manuscript folder using the `manuscript.qmd` file. This file contains the abstract, background information on the dataset, a summary of the exploratory and statistical analyses, and conclusion with strengths and limitations of the study. 

* Explore the `Supplementary-Material.qmd` file in the products > manuscript > supplement folder to find exploratory figures and plots for the three other outcome variables that were not explored in depth in this study. This file also contains more information on our data cleaning process and study methods. 

* The assets folder contains our bibliography in the `dataanalysis-references.bib` file and other files to ensure the template renders correctly. 



