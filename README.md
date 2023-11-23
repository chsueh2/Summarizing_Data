# Summarizing Data

Summarize Student Data and World Development Data from the UCI machine learning repository using pandas and matplotlib.


Key features:

- Exploratory data analysis (EDA)
- One-way, Two-way and Three-way Contingency Tables
- Conditional Two-way Table
- Stacked Bar Graph and Side-by-Side Bar Graph
- Correlation matrix
- Histogram, Kernel Density Plot, Boxplot and Scatterplot
- Line Charts


Modules used:

- `numpy`: Python library used for working with arrays
- `pandas`: data manipulation and analysis. In particular, it offers data structures and operations for manipulating numerical tables and time series.
- `matplotlib.pyplot`: plotting library for creating static, animated, and interactive visualizations
- `itertools`: functions creating iterators for efficient looping

## Project Report

[Project report](https://htmlpreview.github.io/?https://raw.githubusercontent.com/chsueh2/NFL_pandas-on-Spark/main/NFL.html) ([Jupyter Notebook](./Summarizing_Data.ipynb))

The analysis results with theoretical backgrounds are included.

Chien-Lan Hsueh (chienlan.hsueh at gmail.com)

## Overview and Project Goal

To illustrate the ease of parallelization with Spark, we can now update an earlier MapReduce algorithm to run on Spark with far fewer steps required. Previously, we had to read in the large scores dataset, subset based on the value of season, then reread these datasets as an iterable list for the map and reduce functions. Now, we can simply use a pandas on spark dataframe to iterate over the values of seasons and parallelize our earlier computations.

## Workflow

1. Preparation
   - Load module
   - Set up configuration to run Spark
   - define aggregation function to work on data (pyspark.pandas.DataFrame)
   - Read in NFL data (with a quick inspection)
1. Student Data
   - Summarize categorical variables
   - Summarize numerical variables
1. World Development Data
   - summarize the data
   - How the access to clean fuels and technologies for cooking has changed over time in Arab world (ARB)?
   - How the access to electricity has changed over time in the following regions?
   - How the access to electricity has changed over time in rual and uraban areas in Arab world?