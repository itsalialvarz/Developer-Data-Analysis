# Developer Data Analysis: 2024 Stack Overflow Survey

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/itsalialvarz/Developer-Data-Analysis/blob/main/Developer_Data_Analysis_Project.ipynb)
![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458)
![Plotly](https://img.shields.io/badge/Plotly-Interactive%20Viz-3F4F75)


**Author:** Allison Ceballos Alvarez\
**Date:** November, 2025

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect_with_me-blue?style=flat&logo=linkedin)](https://www.linkedin.com/in/allison-ceballos-alvarez/)

---

This project analyzes the **2024 Stack Overflow Developer Survey** (65,000+ responses) to identify key trends in developer demographics, technology preferences, and compensation drivers. The goal is to provide a comprehensive profile of the modern developer and uncover what factors actually correlate with higher pay.

The analysis is performed in a single Jupyter Notebook (`.ipynb`) and includes all steps from data loading and cleaning to exploratory data analysis (EDA), visualization, and conclusion.

---

## How to View This Project

**Note:** GitHub cannot render the interactive Plotly visualizations used in this analysis. To view the full report with interactive charts, please use one of the links below:

### 1. Static HTML Version
**[View Full Analysis (HTML)](https://itsalialvarz.github.io/Developer-Data-Analysis/Developer_Data_Analysis_Project.html)**
*Best for quick viewing. Shows all code, text, and interactive plots in the browser.*

### 2. Interactive Google Colab
**[Run in Google Colab](https://colab.research.google.com/github/itsalialvarz/Developer-Data-Analysis/blob/main/Developer_Data_Analysis_Project.ipynb)**
*Best for testing the code. Opens a live environment where you can execute the analysis.*

### 3. NBViewer
**[View in NBViewer](https://nbviewer.org/github/itsalialvarz/Developer-Data-Analysis/blob/main/Developer_Data_Analysis_Project.ipynb)**
*Alternative renderer if the HTML version is unavailable.*

---

## Table of Contents

1.  [Key Questions & Objectives](#key-questions--objectives)
2.  [Dataset](#dataset)
3.  [Tools and Libraries](#tools-and-libraries)
4.  [Key Findings](#key-findings)
5.  [Limitations & Next Steps](#limitations--next-steps)

---

## Key Questions & Objectives

This analysis seeks to answer several key questions:

1.  **The 2024 Developer Profile:** Who is the "typical" developer?
2.  **The Developer's Toolkit:** What are the most used and most desired technologies in 2024?
3.  **Compensation & Career:** What factors correlate most strongly with salary?, How does compensation vary by experience level and role? and Which technologies are associated with the highest paying positions?

---

## Dataset

This project uses the official **2024 Stack Overflow Developer Survey public dataset**.

* **Source:** [Stack Overflow Developer Survey 2024](https://survey.stackoverflow.co/2024/)
* **Direct Download:** [2024 Full Data Set (CSV)](https://cdn.sstatic.net/insights/survey/2024/survey_results_public.csv)
* **Schema:** [2024 Survey Schema (CSV)](https://cdn.sstatic.net/insights/survey/2024/survey_results_schema.csv)

---

## Tools and Libraries

This analysis was conducted using Python and the following libraries:

* **Data Manipulation:** `pandas`, `numpy`
* **Visualization:** `plotly.express`, `plotly.graph_objects`, `seaborn`, `matplotlib`
* **Utilities:** `re` (Regular Expressions for data cleaning)

---

## Key Findings

* `The Developer Profile:` The typical 2024 developer is 33 years old, holds a Bachelor's degree, and works in a Hybrid role, followed by Remote work. Geographic concentration remains strong in the USA, Germany, and India, representing over one third of responses.

* `The Developer's Toolkit:` JavaScript, SQL, Python, and HTML/CSS remain foundational technologies with highest current usage. However, developer interest has shifted toward Rust, Go, signaling industry movement toward systems languages, performance optimization, and data driven applications.

* `Compensation Dynamics:` The salary analysis reveals three critical findings:
1. Specialization over popularity: The highest paying languages (Erlang, Clojure) and roles (Senior Executive, Security) are not the most common, demonstrating that niche expertise commands premium compensation.
2. Early career acceleration: Salary growth is most dramatic in the first 10-12 years, increasing from ~$45K to over $100K
3. Depth over range: Technology Range Metrics (2.5.2) showed zero correlation between number of technologies known and salary, proving that deep expertise in high value specializations drives compensation, not range.

## Limitations & Next Steps

### Limitations

* `Salary Data Scarcity:` Analysis used 20,903 validated salary responses (35.5% of dataset) between $10K-$500K, ensuring reliability but potentially limiting generalizability to the full developer population.

### Next Steps

* `Predictive modeling:` Build a machine learning model using experience, role, education, and skill features to predict salary, enabling developers to estimate compensation for different career paths.

* `Remote work compensation analysis:` Conduct statistical testing to determine whether Remote, Hybrid, or In-person arrangements correlate with salary differences after controlling for experience, role, and location.