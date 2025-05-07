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

# Data cleaning

Data cleaning (also known as data cleansing) is the process of identifying and correcting (or removing) inconsistencies, errors and inaccuracies within a dataset. In a data science or data analysis project, this process is fundamental in ensuring a reliable and effective analysis, since it lands at the beginning of the pipeline. Data cleaning ensures that the data is accurate, consistent, and reliable.

In essence, data cleaning involves identifying and resolving flaws within datasets by correcting, removing, or modifying records to meet quality standards suitable for analysis. It plays a critical role in data preprocessing and significantly influences how data will be modeled and interpreted.

As an old commercial once said, "Power is nothing without control". The same concept applies here. We can be the best data scientist, business analyst, AI engineer, statistician (or whatever role you prefer), but if we don't have high-quality, clean and consistent data, all our models and predictions are worthless and completely useless. 

### Why Data Cleaning matters

- **Improved data quality**: Cleaning data reduces errors, inconsistencies and missing values, leading to more accurate and reliable analysis.
- **Enhanced efficiency**: High-quality data is easier and quicker to analyze, reducing the time and effort spent managing poor data quality.
- **Better decision-making**: Clean and consistent data provides trustworthy insights, enabling organizations to make well-informed decisions rather than relying on outdated or incomplete data.

### Common Data Quality Issues

Data quality problems may arise from various sources, such as human errors, system failures, or issues during data integration. Typical data quality issues include:

1. **Missing values**: Lack of some data or missing information can result in failure to make the right conclusions and can or else lead to creating a biased result. In order to handle it, different strategies can be adopted:
    - Deleting incomplete records (in case they have minimal impact)
    - Imputing values (by using estimated ones, like the mean, median or mode)
    - Exploiting predictive modeling from the machine learning field to predict the input value
2. **Incorrect data types**: Mismatched data types (e.g., strings in numerical fields) can hinder processing and analysis.
3. **Anomalies and outliers**: Extreme values can skew results and impact statistical accuracy. Detecting and either correcting, removing, or transforming extreme values preserves the accuracy of insights. Sometimes they may be found due to an error in data collection (e.g. if we have the variable `weight` represented in `kg` and we write down an observation in `g`, leading to an enourmous and anomal value with respect to other observations). Another common situation is related to some typos (e.g. we unintentionally add a 0 at the end of a number, thus recording a 10 time higher number). These anomalies are also known as spelling and typographical errors. Fixing typos or inaccurate values often involves validation checks or cross-referencing with trusted sources. 
4. **Duplicate data**: Repeated entries can distort results, metrics and produce skewed results. Identifying and eliminating redundant records ensures data integrity and uniqueness.
5. **Inconsistent formats**: Disparities in formats (e.g., date formats, text casing) complicate data aggregation and comparison. Ensuring uniformity in formats such as dates, addresses, and phone numbers is essential for an easier analysis.

## Challenges in Data Cleaning

When trying to clean our source data, different problems can be faced:

- Large Volumes: Big datasets require scalable tools and efficient methods, due to their sheer size.
- Ongoing Nature: Cleaning is not a one-time task but a continuous process as new data is collected and integrated.
- Data Complexity: Data may come from different sources and have diverse formats: these multiple sources can be hard to reconcile.
