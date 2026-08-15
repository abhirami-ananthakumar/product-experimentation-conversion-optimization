# Dataset

## 1. Dataset Overview

This project uses the **Marketing A/B Testing** dataset published on Kaggle by **FavioVázquez**.

The dataset represents a marketing experiment designed to evaluate whether displaying advertisements leads to a higher conversion rate compared with showing users a Public Service Announcement (PSA).

The experiment contains two groups:

- **Ad Group** — Users who were exposed to advertisements.
- **PSA Group** — Users who were shown a public service announcement and served as the control group.

The primary business question is:

> Does exposure to the advertising campaign significantly improve user conversion?

---

## 2. Source Dataset

**Dataset Name:** Marketing A/B Testing

**Author:** FavioVázquez

**Platform:** Kaggle

**Dataset Link:**  
https://www.kaggle.com/datasets/faviovaz/marketing-ab-testing

**License:** CC0: Public Domain

The original Kaggle dataset contains one CSV file named `marketing_AB.csv` with 7 columns. The dataset is approximately 21.98 MB in size.

---

## 3. Original Dataset Structure

The original dataset contains the following fields:

| Column | Description |
|---|---|
| `Index` | Row index |
| `user id` | Unique identifier assigned to each user |
| `test group` | Experiment group: `ad` or `psa` |
| `converted` | Indicates whether the user converted |
| `total ads` | Total number of advertisements seen by the user |
| `most ads day` | Day on which the user saw the highest number of advertisements |
| `most ads hour` | Hour during which the user saw the highest number of advertisements |

---

## 4. Dataset Purpose

The dataset is used to perform an end-to-end product experimentation analysis.

The analysis focuses on:

- Comparing conversion rates between experiment groups
- Measuring the effect of advertising exposure
- Understanding advertisement exposure patterns
- Identifying conversion patterns by day and hour
- Performing statistical hypothesis testing
- Determining whether the observed difference is statistically significant
- Supporting a business decision on whether the advertising campaign should be continued or scaled

---

## 5. Data Preparation

The original Kaggle dataset was inspected and prepared before analysis.

The preparation process included:

- Initial dataset inspection
- Data type validation
- Duplicate record checking
- Missing value checking
- Unique value validation
- Categorical value validation
- Conversion field validation
- Experiment group validation
- Creation of analysis-ready fields where required
- Removal of unnecessary fields from the analysis dataset

The cleaned dataset was then saved as a separate CSV file to preserve the original source data.

---

## 6. Cleaned Dataset

The cleaned dataset is stored in this folder as:

`marketing_AB_cleaned.csv`

The cleaned CSV is the analysis-ready version of the original Kaggle dataset.

It is used as the primary input for:

- Exploratory Data Analysis
- A/B Test Analysis
- Statistical Testing
- Visualization
- Business Recommendations

---

## 7. Cleaned Dataset Structure

The cleaned dataset retains the relevant variables required for the analysis.

| Column | Description |
|---|---|
| `user_id` | Unique user identifier |
| `test_group` | Experiment group: `ad` or `psa` |
| `converted` | Conversion indicator |
| `total_ads` | Total advertisements seen by the user |
| `most_ads_day` | Day with the highest advertisement exposure |
| `most_ads_hour` | Hour with the highest advertisement exposure |

The cleaned column names use a consistent naming convention to make analysis easier in Python.

---

## 8. Key Dataset Characteristics

The experiment contains two substantially different group sizes:

| Experiment Group | Users |
|---|---:|
| Ad | 564,577 |
| PSA | 23,524 |
| **Total** | **588,101** |

The dataset contains a binary conversion outcome:

- `1 / True` — User converted
- `0 / False` — User did not convert

This structure makes the dataset suitable for conversion-rate analysis and a two-proportion statistical test.

---

## 10. Data Privacy

The dataset is publicly available on Kaggle and is used for educational and portfolio analysis purposes.

The project does not attempt to identify individual users or derive personally identifiable information.

---

## 12. Source Attribution

Original dataset:

**Marketing A/B Testing — FavioVázquez**

Kaggle:  
https://www.kaggle.com/datasets/faviovaz/marketing-ab-testing

The original dataset remains the source of the data used in this project. The cleaned CSV is a prepared version created specifically for analysis.
