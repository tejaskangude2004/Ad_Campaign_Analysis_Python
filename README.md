# Ad_Campaign_Analysis_Python
The primary goal of this research is to find which ad campaign is working well for sales.
# Ad Campaign Analysis: Facebook vs. Instagram

## Project Overview

This project analyzes the performance of Facebook and Instagram advertising campaigns to determine which platform generates higher customer conversions. Using Python for data analysis and Welch's Independent Samples t-test for statistical inference, the project compares campaign effectiveness and provides data-driven business insights.

Project Type: Marketing Analytics | Statistical Analysis | Data Analysis

---

## Objectives

* Compare the performance of Facebook and Instagram advertising campaigns.
* Analyze the relationship between ad views, clicks, and conversions.
* Categorize campaigns based on conversion performance.
* Perform statistical hypothesis testing to determine whether the difference in conversions is significant.
* Identify the platform that provides better marketing performance.

---

## Dataset Information

The dataset contains 365 observations and 9 features.

### Features

* Date
* Facebook Ad Views
* Facebook Ad Clicks
* Facebook Ad Conversions
* Facebook Ad Cost Per Day
* Instagram Ad Views
* Instagram Ad Clicks
* Instagram Ad Conversions
* Instagram Ad Cost Per Day

Note: This dataset was synthetically generated for educational and analytical purposes.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy
* Jupyter Notebook

---

## Exploratory Data Analysis (EDA)

The following preprocessing steps were performed:

* Imported the dataset using Pandas
* Checked dataset structure using `info()`
* Generated summary statistics using `describe()`
* Verified missing values
* Renamed columns using snake_case
* Created new conversion category columns for Facebook and Instagram

---

## Data Analysis

### 1. Correlation Analysis

Relationship between advertisement clicks and conversions:

| Platform  | Correlation |
| --------- | ----------: |
| Facebook  |    **0.86** |
| Instagram |    **0.79** |

Both platforms show a strong positive relationship between clicks and conversions. Facebook demonstrates a stronger correlation, suggesting clicks are more likely to convert into successful customer actions.

---

### 2. Distribution Analysis

Histograms were created to visualize the distributions of:

* Advertisement Clicks
* Advertisement Conversions

Although the distributions alone were not sufficient to draw conclusions, they provided valuable insight into campaign behavior.

---

### 3. Conversion Category Analysis

Campaigns were grouped into four conversion ranges:

* Less than 200
* 200–400
* 400–600
* More than 600

| Conversion Category | Facebook | Instagram |
| ------------------- | -------: | --------: |
| Less than 200       |        0 |       340 |
| 200–400             |        2 |        25 |
| 400–600             |       78 |         0 |
| More than 600       |      285 |         0 |

This comparison clearly shows that Facebook campaigns consistently achieved higher conversion ranges, whereas most Instagram campaigns remained below 200 conversions.

---

## Statistical Analysis

### Welch's Independent Samples t-test

### Null Hypothesis (H₀)

The average Facebook and Instagram ad conversions are equal.

### Alternative Hypothesis (H₁)

The average Facebook and Instagram ad conversions are different.

### Test Results

| Metric         |             Value |
| -------------- | ----------------: |
| Facebook Mean  |        **788.53** |
| Instagram Mean |        **134.28** |
| t-statistic    |         **58.94** |
| p-value        | **1.28 × 10⁻¹⁹⁸** |

### Interpretation

Since the p-value is significantly smaller than 0.05, the null hypothesis is rejected.

The statistical evidence confirms that Facebook advertisements generate significantly higher average conversions than Instagram advertisements.

---

## Key Insights

* Facebook campaigns achieved substantially higher conversion rates.
* Facebook exhibited a stronger click-to-conversion relationship.
* Instagram campaigns were primarily concentrated in the lowest conversion category.
* Statistical testing confirmed that the observed difference was highly significant and not due to random variation.

---

## Business Recommendation

Based on this analysis:

* Allocate a larger portion of the advertising budget to Facebook campaigns.
* Continue optimizing Instagram campaigns to improve conversion efficiency.
* Monitor campaign performance regularly using statistical testing instead of relying solely on descriptive metrics.

---

## How to Run

```bash
git clone https://github.com/yourusername/Ad-Campaign-Analysis.git

cd Ad-Campaign-Analysis

pip install -r requirements.txt

jupyter notebook
```

---

## Python Libraries

```python
pandas
numpy
matplotlib
seaborn
scipy
```

---

## Conclusion

This project demonstrates how statistical analysis can support marketing decision-making. By combining exploratory data analysis with Welch's Independent Samples t-test, the analysis provides strong evidence that Facebook advertising campaigns significantly outperform Instagram campaigns in terms of customer conversions.

---

## Author

Tejas Kangude

Aspiring Data Analyst

---

⭐ If you found this project useful, consider giving it a star on GitHub!
