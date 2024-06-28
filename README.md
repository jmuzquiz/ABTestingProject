# A/B Testing Analysis

## Table of Contents
1. [Introduction](#introduction)
2. [Background](#background)
   - [Dataset Source](#dataset-source)
   - [Dataset Description](#dataset-description)
3. [Google Colab Notebook](#google-colab-notebook)
4. [Project Overview](#project-overview)
   - [Objectives](#objectives)
   - [Tools I Used](#tools-i-used)
1. [Introduction](#introduction)
2. [Dataset Description](#dataset-description)
3. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
4. [A/B Testing Analysis](#ab-testing-analysis)
5. [Results](#results)
6. [Conclusion](#conclusion)
7. [Code](#code)
8. [Dependencies](#dependencies)
9. [Usage](#usage)

## Introduction
📊 Dive into the world of A/B testing analysis with this project! We're exploring how different user exposures—ads versus PSAs—affect conversion rates and simulated revenue. Join me in analyzing the data to derive meaningful insights that drive strategic business decisions.

## Background
### Dataset Source
The dataset used in this project was sourced from Kaggle link*. It comprises data related to a marketing A/B testing scenario aimed at evaluating the effectiveness of advertising campaigns. A majority of the people in the sample were exposed to ads (the experimental group). And a small portion of people (the control group) instead saw a Public Service Announcement (PSA) in the exact size and place the ad would normally be. 

### Dataset Description
The dataset contains the following columns:
- `Index`: Row index
- `user id`: Unique identifier for each user
- `test group`: Specifies whether the user saw an advertisement ("ad") or a Public Service Announcement ("psa")
- `converted`: Indicates whether the user made a purchase (True) or not (False)
- `total ads`: Total number of advertisements seen by each user.
- `most ads day`: Day of the week when the user viewed the highest number of advertisements
- `most ads hour`: Hour of the day when the user viewed the highest number of advertisements

## Google Colab Notebook

This notebook contains the Python code used for the A/B testing analysis in this project. Click [here](link-to-your-notebook-file)* to view the notebook.

The notebook includes data preprocessing steps, visualizations, statistical analysis, and simulations related to evaluating the effectiveness of advertising campaigns using A/B testing.

## Project Overview
This project focuses on conducting an A/B testing analysis to evaluate the impact of ad exposure on conversion rates and simulated revenue. The primary objective is to gain familiarity with A/B testing methodologies and leverage data analysis techniques to assess the significance of experimental results. By simulating revenue based on conversion metrics and applying rigorous statistical tests, the project aims to uncover valuable insights that can guide strategic marketing decisions. Additionally, this project offered me a valuable opportunity to demonstrate my proficiency in Python, showcasing advanced analytical skills and the ability to create impactful data visualizations using key Python packages.

### Objectives
1. Identify peak days and hours of ad exposure for users.
2. Determine the day of the week and time of day with the highest conversion rates.
3. Assess if conversion rates vary significantly based on the day or hour of ad exposure.
4. Compare conversion rates between users exposed to ads and those in the control group.
5. Explore how the number of ads seen influences conversion likelihood.
6. Analyze simulated revenue differences between users who converted and those who did not.
7. Calculate the total revenue generated from users who converted during the ad campaign.

### Tools I Used
For my A/B testing analysis project, I utilized the following tools and platforms:

- **Python**: Used extensively for data preprocessing, statistical analysis, and creating visualizations.
- **Google Colab**: Leveraged for its cloud-based Python environment, ideal for running Jupyter notebooks and collaborating on projects.
- **Git and GitHub**: Employed for version control, enabling me to track changes, manage project iterations, and share my work with others.
- **NumPy and Pandas**: Essential Python libraries for data manipulation, allowing me to handle and analyze the dataset efficiently.
- **Matplotlib and Seaborn**: Used for data visualization, helping me create informative plots and charts to illustrate findings.
- **SciPy**: Utilized for statistical tests such as t-tests and Mann-Whitney U tests, crucial for evaluating experimental results.
  
This project enabled me to leverage my proficiency in Python programming, collaborative tools like Google Colab and GitHub, and essential data analysis and visualization libraries. These tools were instrumental in conducting rigorous A/B testing analysis and deriving meaningful insights from the dataset.


------------
## Project Structure
1. **Data Preprocessing** / exploratory data anlayis?
   - Cleaning and preparing the dataset for analysis.
   - Handling missing values and ensuring data integrity.

2. **Univariate Analysis**
   - Exploring individual variables such as `test group`, `converted`, `total ads`, `most ads day`, and `most ads hour`.
   - Visualizing distributions, summary statistics, and identifying any outliers.

3. **Bivariate Analysis**
   - Investigating relationships between `converted` and other variables.
   - Analyzing how variables like `test group` or `total ads` relate to conversion rates.

4. **Statistical Tests**
   - Conducting hypothesis tests (e.g., t-tests, Mann-Whitney U tests) to assess the significance of observed differences.
   - Interpreting p-values and making conclusions based on statistical significance.

5. **Simulated Revenue Analysis**
   - **Data Modification:**
     - Simulating a `simulated_revenue` column based on conversion status and ad exposure.
   - **Univariate Analysis:**
     - Examining the distribution and summary statistics of `simulated_revenue`.
   - **Bivariate Analysis:**
     - Exploring relationships between `converted` and `simulated_revenue`.
     - Analyzing how `simulated_revenue` varies across different factors like `test group` or `total ads`.
   - **Statistical Tests:**
     - Performing tests to compare `simulated_revenue` between converted and non-converted groups.
     - Discussing the implications for potential business decisions.

## Insights and Interpretation
- Summarize the key findings from both the initial A/B testing analysis and the simulated revenue analysis.
- Interpret the results in the context of the project's objectives and discuss their theoretical implications for business strategies.

## Conclusion
- Reflect on the project's goals and what was achieved through the analysis.
- Discuss any limitations encountered and opportunities for further exploration or refinement.

## Visualizations and Code
- Include visualizations (e.g., plots, charts) that highlight key insights.
- Provide snippets of code used for data preprocessing, analysis, and statistical tests.

------

# A/B Testing Analysis Project README

## Overview
This project aims to conduct an A/B testing analysis to evaluate the effectiveness of an advertising campaign in increasing user conversion rates. The analysis focuses on comparing two groups: one exposed to advertisements (experimental group) and another exposed to Public Service Announcements (PSAs) or no exposure (control group). The primary goal is to determine if there is a statistically significant difference in conversion rates between these groups.

## Data Description
The dataset used in this analysis includes the following variables:
- **test group**: Indicates whether users were in the experimental (ad exposure) or control (PSA/no exposure) group.
- **converted**: Binary variable indicating if the user converted (True) or did not convert (False).
- **total ads**: Number of ads each user was exposed to during the campaign.
- **most ads day**: Day of the week when the user saw the most ads.
- **most ads hour**: Hour of the day when the user saw the most ads.

## Project Structure
1. **Data Preprocessing**
   - Cleaned and prepared the dataset, handling missing values and ensuring data integrity.
   - Converted categorical variables into appropriate formats for analysis.

2. **Exploratory Data Analysis**
   - Conducted univariate analysis to understand the distribution of variables.
   - Visualized relationships between variables using histograms, bar plots, and scatter plots.

3. **Hypothesis Testing**
   - **Assumptions Check:**
     - Tested for normality and equality of variances using Shapiro-Wilk and Levene's tests.
   - **Statistical Tests:**
     - Used independent two-sample t-tests to compare conversion rates between the experimental and control groups.
     - Applied non-parametric Mann-Whitney U tests as alternatives when assumptions for t-tests were not met.

4. **Simulated Revenue Analysis**
   - **Data Transformation:**
     - Simulated a `simulated_revenue` column based on conversion status and total ads exposure.
   - **Revenue Analysis:**
     - Analyzed the distribution and statistical significance of simulated revenue differences between converted and non-converted groups.

5. **Insights and Interpretation**
   - Summarized findings from the A/B testing and simulated revenue analyses.
   - Interpreted results to derive theoretical business insights, including implications for marketing strategies and revenue generation.

## Conclusion
- Concluded with insights into the effectiveness of the advertising campaign based on statistical evidence.
- Discussed limitations of the analysis and suggestions for future research or improvements.

## Visualizations and Code
- Included visualizations such as histograms, box plots, and statistical tests' output.
- Provided snippets of Python code used for data preprocessing, analysis, and visualization.

## Future Steps
- Suggested next steps for further exploring the data or refining the analysis methodology.
- Proposed additional experiments or data collection efforts to strengthen the analysis conclusions.

## Acknowledgments
This project was inspired by a YouTube tutorial on analyzing A/B testing data. While the initial analysis approach followed the tutorial, additional visualizations and a simulated revenue column were added to further explore the dataset and derive business insights.

Tutorial Link: YouTube - Analyzing A/B Testing Data

## Future Steps
- Outline potential next steps for enhancing the analysis or applying findings in real-world scenarios.
- Consider additional experiments or refinements to improve the accuracy and reliability of results.

