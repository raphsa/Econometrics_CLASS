---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Stata introduction

Stata is a powerful, multipurpose statistical software package used primarily for data analysis, data management, and graphics.

Stata allows to handle large datasets efficiently and provides data cleaning tools like dealing with missing values and variable recording.

From the statistical aspects, Stata provides all the tests to inference on different quantities. It supports cross-section data, panel data and time series.

## Stata commands

Here you can find a list of the main commands you will need to clean your dataset and to perform statistical analysis:

###### Data management

- `use`: Loads a dataset. Even `u` is accepted.
- `save`: Saves the current dataset.
- `import`/`export`: Imports or exports data (in .csv, .xls, etc.).
- `list`: Lists data in the Data Editor.
- `browse`: Opens Data Browser.
- `edit`: Opens Data Editor in edit mode.
- `gen`: Creates a new variable. Even `generate` is accepted.
- `replace`: Modifies an existing variable.
- `drop`: Deletes variables or observations.
- `keep`: Keeps specific variables or observations.
- `sort`: Sorts data by one or more variables.
- `order`: Reorders variables.
- `rename`: Renames a variable.
- `merge`: Combines datasets by key variables.
- `append`: Stacks datasets vertically.
- `reshape`: Restructures dataset.
- `clear`: Clears the current dataset from memory.
- `set more off`/`set more on`: Controls whether Stata pauses after output fills the screen.
- `recode`: Changes the values of a variable based on specified rules.


###### Descriptive statistics

- `sum`: Shows summary statistics (like mean, SD, min, max). Even `summarize` is accepted.
- `tab`: Shows the frequency tables. Even `tabulate` is accepted.
- `codebook`: Provides detailed summary of variables.
- `describe`: Provides metadata (like variable names, types, etc.).

###### Statistical analysis

- `regress`: Performs linear regression.
- `logit`/`probit`: Performs logistic and probit regression.
- `ttest`: Performs T-tests.
- `anova`: Performs Analysis of Variance.
- `corr`: Provides the correlation matrix. Even `correlate` is accepted.
- `tabstat`: Provides customizable summary statistics.
- `xtreg`: Performs panel data regression.
- `stcox`: Performs survival analysis.
- `sem`: Performs structural equation modeling.
- `factor`: Performs factor analysis.
- `pca`: Performs principal component analysis.
- `xtset`: Declares a panel data structure. Needed if we want to work with panel data (like in `xtreg` case).

###### Graphing

- `graph`: Is the base for many graphs.
- `histogram`: Provides the histogram of a variable.
- `scatter`: Provides the scatter plot of two variables.
- `line`: Provides the line graph of two variables.
- `boxplot`: Provides the boxplot of a variable.
- `twoway`: Combines multiple graph types.

###### Programming and automation

- `do`: Runs a do-file.
- `log using`: Records output in a log file.
- `foreach`/`forvalues`: Loops over lists or ranges.
- `if`/`in`: Performs if statements for conditional execution.
- `macro`: Defines macros.
- `capture`: Runs commands and ignore errors.
- `assert`: Checks data integrity.
- `bys`: Applies a command by groups defined by one or more variables. Even `by varlist:` is accepted.
- `by`: Applies commands by groups but requires data to be sorted beforehand.

###### Help and support

- `help`: Views help for a command (e.g., `help gen`).
- `search`: Searches for commands and documentation.
- `update`: Checks for software updates.