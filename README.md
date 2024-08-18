# Life Expectancy Prediction Project

## Overview

This project was developed as part of the DSC 532 – Statistical Learning course in the Master’s program of Data Science at University of Cyprus. The objective was to predict life expectancy at birth using various statistical and machine learning models implemented in R. The project explores a wide array of factors, from health indicators to economic and social variables, impacting life expectancy across 179 countries from 2000 to 2015. The goal was to uncover critical influences on life expectancy and offer actionable insights for policymakers to enhance longevity.

## Project Structure

- **Introduction**: Overview of the project’s predictive goals and the importance of understanding the factors influencing life expectancy.
- **Data Preprocessing**: Data preparation steps including data type conversion, handling missing values, and splitting the dataset into training and test sets.
- **Exploratory Data Analysis**: Visualizations and analysis of key factors such as economic status, region, alcohol consumption, and GDP per capita.
- **Feature Selection**: Selection of the most relevant predictors using techniques like Best Subset Selection and Cross-Validation.
- **Modeling**: Application of Linear Regression and Random Forest Regression models using R. Includes model evaluation metrics.
- **Conclusion**: Summary of findings, key predictors, and recommendations for policymakers.

## Data Sources

- **Kaggle**: The primary dataset was sourced from a Kaggle competition.
- **World Health Organization (WHO) Global Health Observatory**: Supplementary data on health metrics.
- **World Bank Databank**: Additional economic and social indicators.

## Usage

1. **Data Preprocessing**: Run the R Markdown file to preprocess the data by converting data types, handling missing values, and splitting the dataset.
2. **Exploratory Data Analysis**: Use the provided R code to visualize and analyze the data.
3. **Modeling**: Train and evaluate the predictive models using the R Markdown provided.
4. **Prediction**: Generate predictions for life expectancy based on the trained models.

## Dependencies

- R version 4.3.3 or higher
- `ggplot2`
- `dplyr`
- `MASS`
- `DescTools`
- `nortest`
- `moments`
- `reshape2`
- `mice`
- `leaps`
- `corrplot`
- `GGally`
- `glmnet`
- `randomForest`
- `boot`

## Installation

To install the required R packages, you can run:

```r
list.of.packages <- c("ggplot2", "dplyr", "MASS", "DescTools", "nortest", "moments", "reshape2",
"mice", "leaps", "corrplot", "GGally", "glmnet", "randomForest", "boot")
new.packages <- list.of.packages[!(list.of.packages %in% installed.packages()[, "Package"])]
# Install them in case they are not already
if (length(new.packages)) install.packages(new.packages)
# Load packages
invisible(lapply(list.of.packages, library, character.only = TRUE))

