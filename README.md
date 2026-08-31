# 🦠 COVID-19 Data Analysis

### Turning raw COVID-19 case data into an analysis-ready dataset

This project focuses on **cleaning and analyzing a real-world COVID-19 case dataset from Canada**.

Instead of directly working with the raw data, I first inspected the dataset, identified missing and inconsistent values, standardized important fields, removed unnecessary information, and created a separate cleaned dataset for analysis.

The main goal of this project was to understand how much work is required to turn **messy real-world data into reliable, structured data for analysis**.

---

## 📌 Project Overview

Real-world datasets are rarely ready for analysis.

The original COVID-19 dataset contained missing values, inconsistent age representations, incomplete demographic information, and fields that were not useful for the analysis.

I worked on the dataset through the following process:

**Raw Data → Data Inspection → Data Cleaning → Data Validation → Clean Dataset → Analysis**

The cleaned dataset is saved as:

```text
out.csv
```

---

## 🎯 Objectives

* Understand the structure and quality of the raw dataset.
* Identify missing and inconsistent values.
* Clean and standardize important data fields.
* Remove unnecessary or unusable columns.
* Create an analysis-ready dataset.
* Explore COVID-19 cases based on demographic, geographic and temporal information.
* Understand the practical challenges involved in real-world data preprocessing.

---

## 📂 Dataset

The repository contains two versions of the dataset:

### 1. Raw Dataset

```text
raw data.csv
```

This is the original dataset before applying any transformations.

### 2. Cleaned Dataset

```text
out.csv
```

This is the dataset after cleaning, standardization and preprocessing.

Keeping both versions makes the transformation process **transparent and reproducible**.

---

## 🧹 Data Cleaning Process

The major cleaning steps included:

### 1. Removing unusable information

Columns that contained no useful information or were not required for the intended analysis were removed.

### 2. Standardizing age groups

Different representations of younger age groups were standardized into a common age category such as:

```text
0-19
```

while preserving the existing adult age ranges.

This makes age-based analysis more consistent.

### 3. Handling missing values

The raw dataset contained values such as:

```text
Not Reported
NULL
```

These values were identified and handled during preprocessing.

For selected fields, missing categories were replaced according to the cleaning rules used in the analysis.

> **Note:** These replacements are preprocessing assumptions and should not be interpreted as confirmed patient information.

### 4. Removing unnecessary fields

Fields that were not useful for the final analysis were removed from the cleaned dataset.

This helps keep the dataset focused and easier to work with.

### 5. Data validation

After cleaning, the dataset was checked for:

* Missing values
* Duplicate records
* Incorrect categories
* Column structure
* Data consistency

---

## 📊 Dataset Snapshot

The cleaned dataset contains approximately:

| Feature                         |  Value |
| ------------------------------- | -----: |
| Records                         | 50,982 |
| Province / territory categories |     13 |
| Health regions                  |     85 |
| Age groups                      |      9 |
| Sex categories                  |      2 |
| Reporting weeks                 |     15 |

The reporting period covers:

**January 25, 2020 – April 28, 2020**

---

## 🔎 Analysis Performed

The cleaned dataset can be used to explore several dimensions of COVID-19 cases.

### 🌎 Geographic Analysis

* Province-wise case distribution
* Health-region level analysis
* Comparison of reported cases across regions

### 👥 Demographic Analysis

* Age-group distribution
* Sex distribution
* Comparison between demographic groups

### 📅 Temporal Analysis

* Daily reported cases
* Weekly case trends
* Changes in reported case volume over time

### 🧪 Data Quality Analysis

* Missing-value analysis
* Category standardization
* Duplicate detection
* Raw vs cleaned dataset comparison

---

## 💻 Technologies Used

| Technology                     | Purpose                                    |
| ------------------------------ | ------------------------------------------ |
| **Python**                     | Main programming language                  |
| **Pandas**                     | Data cleaning, transformation and analysis |
| **NumPy**                      | Numerical operations                       |
| **Matplotlib**                 | Static data visualization                  |
| **Plotly**                     | Interactive visualization                  |
| **Jupyter Notebook / VS Code** | Development and analysis                   |
| **Git & GitHub**               | Version control and project management     |

---

## 🔄 Data Processing Workflow

```text
                 Raw COVID-19 Dataset
                         │
                         ▼
                  Data Inspection
                         │
                         ▼
                 Identify Data Issues
                         │
             ┌───────────┼───────────┐
             ▼           ▼           ▼
        Missing Data  Inconsistent  Unnecessary
                       Categories     Fields
             │           │           │
             └───────────┼───────────┘
                         ▼
                   Data Cleaning
                         │
                         ▼
                 Data Standardization
                         │
                         ▼
                   Data Validation
                         │
                         ▼
                  Cleaned Dataset
                      out.csv
                         │
                         ▼
               Exploratory Analysis
                         │
                         ▼
                  Insights & Charts
```

---

## 💡 Key Learning

The biggest takeaway from this project was that **data analysis starts long before visualization**.

Working with the raw dataset helped me understand how real-world data can contain:

* Missing information
* Inconsistent categories
* Unnecessary fields
* Ambiguous values
* Data-quality issues

Cleaning these problems before analysis is essential because **poor-quality input data can lead to misleading results**.

This project therefore helped me strengthen my practical skills in:

* Data preprocessing
* Data cleaning
* Pandas
* Exploratory Data Analysis
* Data validation
* Data visualization
* Handling real-world datasets

---

## ⚠️ Data Quality & Limitations

This dataset represents **reported COVID-19 cases**, not necessarily the complete number of infections in the population.

Some records contain `Not Reported` or incomplete information. Certain missing values were handled using explicit preprocessing rules.

Therefore, the cleaned dataset should be used for:

* Educational purposes
* Exploratory data analysis
* Data-processing demonstrations
* Learning data engineering and analytics workflows

It should **not** be treated as a source for medical or epidemiological decisions.

---

## 🚀 Future Improvements

I plan to extend this project by:

* Building an automated ETL pipeline
* Adding automated data-quality checks
* Creating an interactive Streamlit dashboard
* Adding more detailed statistical analysis
* Adding unit tests for data-cleaning functions
* Making the preprocessing pipeline reproducible
* Exploring machine-learning applications on the cleaned dataset

---

## 👨‍💻 Project Focus

This project represents a practical step toward **Data Engineering and Machine Learning**.

Rather than only focusing on the final visualization, I focused on the complete data journey:

> **Understand → Clean → Validate → Analyze → Visualize**

The project demonstrates my ability to work with imperfect real-world data and transform it into a structured dataset that can support further analysis and machine-learning workflows.

---

## 📁 Repository Structure

```text
COVID-19-Data-Analysis/
│
├── README.md
├── raw data.csv
└── out.csv
```

More analysis scripts, notebooks and visualizations can be added as the project evolves.

---

## 📜 Disclaimer

This is an educational data-analysis project based on a publicly available COVID-19 dataset from Canada.

The analysis is intended to demonstrate **data cleaning, preprocessing and exploratory analysis techniques** and should not be interpreted as medical or official epidemiological guidance.
