# NYC DCWP Consumer Complaints Analysis

## 📌 Project Overview

This project performs an end-to-end Exploratory Data Analysis (EDA) of consumer complaints received by the New York City Department of Consumer and Worker Protection (DCWP). Using Python, the project explores complaint patterns, intake channels, complaint outcomes, refund amounts, and processing times to understand how complaints are distributed and resolved.

The workflow covers data inspection, cleaning, preprocessing, statistical analysis, and visualization. The analysis is organized around questions, with charts and interpretations used to communicate findings from the dataset.

## 🎯 Objectives

- Clean and validate the consumer complaints dataset while documenting preprocessing decisions.
- Investigate missing values, duplicate records, data types, and data quality.
- Perform univariate, bivariate, and multivariate exploratory analysis.
- Compare complaint volumes, intake channels, and complaint results.
- Examine refund amounts and complaint processing times.
- Communicate key findings and develop data-driven recommendations.

## 🗂️ Dataset Description

- **Source:** NYC Department of Consumer and Worker Protection (DCWP) consumer complaints dataset.
- **Format:** CSV.
- **Dataset size after cleaning:** 76,527 rows.
- **Columns:** 29 original columns, with an additional derived feature for processing time.
- **Content:** Consumer complaint records, intake channels, complaint results, dates, and refund-related information.
- **Data types:** Numerical, categorical, and date/time fields.

### Dataset Access

The original and cleaned datasets can be accessed through the links below:

- **Original dataset:** https://drive.google.com/file/d/19zB3hcZVIEW2lQIjyee3RsbWOoyklb1q/view?usp=drive_link
- **Cleaned dataset:** https://drive.google.com/file/d/1_yWsjc_gbLmHmCuMDwO30dP41Id2Y_0V/view?usp=drive_link

*The datasets are hosted externally if their file sizes are unsuitable for direct GitHub upload.*

## 🔧 Project Workflow

### 1. Data Loading and Initial Overview

Loaded the dataset using Pandas and inspected its structure, dimensions, column names, data types, and descriptive statistics. Initial exploration helped establish the dataset's quality and suitability for further analysis.

### 2. Data Cleaning and Preprocessing

- **Missing values:** Examined missing-value patterns and handled them according to the cleaning decisions documented in the notebook.
- **Duplicates:** Checked for duplicate records as part of data quality assessment.
- **Data types:** Converted relevant date columns to appropriate datetime types.
- **Data validation:** Inspected the dataset for consistency and prepared it for analysis.
- **Feature engineering:** Created a `Processing Days` feature using the difference between the result date and intake date.
- **Outlier detection:** Applied the Interquartile Range (IQR) method to the `Refund Amount` column. Identified 216 outlier observations, representing 14.31% of non-missing refund amounts.

### 3. Exploratory Data Analysis

The analysis explores the dataset from multiple perspectives:

| Analysis area | Questions explored |
|---|---|
| Complaint distribution | Which complaint categories and intake channels account for the most records? |
| Complaint outcomes | Which results occur most frequently? |
| Intake channels | How do complaint outcomes vary across intake channels? |
| Refund amounts | How are refund amounts distributed, and are there extreme observations? |
| Processing time | How long does it take for complaints to reach a recorded result? |
| Relationships | What patterns emerge when comparing complaint attributes and outcomes? |

### 4. Data Visualization

The project uses Python visualization libraries to present patterns and relationships in the data. Visualizations include distribution charts, category comparisons, outcome comparisons across intake channels, and other exploratory plots.

Each visualization is accompanied by an explanation of what it shows and why the finding matters.

### 5. Insight Generation

The final stage translates the exploratory results into key insights and recommendations. Interpretations are based on the observed data, including patterns that may be useful for understanding complaint handling and processing.

## 🔍 Key Areas of Analysis

- **Intake channels:** Identified the most common channels through which complaints were received.
- **Complaint results:** Examined the distribution of recorded complaint outcomes.
- **Channel-wise outcomes:** Compared the five most common complaint results across intake channels using within-channel percentages.
- **Refund amounts:** Analysed the distribution of refund amounts and detected outliers using the IQR method.
- **Processing time:** Created a derived feature to investigate the number of days between intake and recorded result dates.

## 💡 Recommendations and Practical Implications

- **Monitor complaint intake channels:** Use channel-wise complaint volumes to understand where complaints are most frequently received and where operational capacity may be needed.
- **Review complaint outcomes:** Examine the most common recorded results to identify areas that may benefit from further investigation.
- **Compare outcomes across channels:** Use within-channel percentages to compare complaint-result patterns without relying only on raw counts.
- **Investigate extreme refund amounts:** Review outliers to determine whether they reflect legitimate high-value cases, unusual records, or potential data quality issues.
- **Monitor processing time:** Use the `Processing Days` feature to explore delays and identify complaint groups that may warrant closer review.
- **Improve data-driven reporting:** Maintain consistent data validation and exploratory reporting to support better understanding of consumer complaint patterns.

## 🛠️ Tools and Technologies

- **Language:** Python
- **Data manipulation:** Pandas, NumPy
- **Visualization:** Matplotlib, Seaborn, Plotly
- **Environment:** Jupyter Notebook
- **Version control:** Git and GitHub

## ▶️ How to Run

1. Clone or download this repository.
2. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn plotly jupyter
   ```

3. Download the dataset using the links in the Dataset Access section.
4. Update the CSV file path in the notebook if needed.
5. Open the notebook in Jupyter Notebook or VS Code.
6. Run all cells from beginning to end.

## 📁 Repository Structure

```text
DCWP-Consumer-Complaints-Analysis/
├── Data_Cleaning.ipynb
├── README.md
└── Dataset files
    └── Access through the Google Drive links above
```



## ✏️ Author

**Ashe Mariya Binu**

Data Analytics | Python | Exploratory Data Analysis
