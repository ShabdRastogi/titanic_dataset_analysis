# Titanic Survival Analysis

## Overview

This project is a part of the **BRL AKGEC Wildcard Task** under the **Machine Learning** domain. The objective is to preprocess the Titanic dataset, perform Exploratory Data Analysis (EDA), engineer useful features, and prepare the dataset for machine learning.

The project demonstrates the complete data preprocessing workflow, including handling missing values, removing unnecessary columns, creating new features, and visualizing important insights from the dataset.

---

## Objectives

- Load and explore the Titanic dataset.
- Identify and handle missing values.
- Remove duplicate records.
- Perform feature engineering.
- Visualize the dataset using different plots.
- Prepare the cleaned dataset for machine learning.

---

## Dataset Information

The dataset contains information about passengers aboard the RMS Titanic.

### Features

| Feature | Description |
|----------|-------------|
| PassengerId | Unique passenger ID |
| Survived | Survival (0 = No, 1 = Yes) |
| Pclass | Passenger class |
| Name | Passenger name |
| Sex | Gender |
| Age | Passenger age |
| SibSp | Number of siblings/spouses aboard |
| Parch | Number of parents/children aboard |
| Ticket | Ticket number |
| Fare | Ticket fare |
| Cabin | Cabin number |
| Embarked | Port of embarkation |

---

## Project Structure

```
Titanic-Survival-Analysis/
│
├── Titanic_survival_analysis.ipynb
├── Titanic_revised.csv
├── Report.docx
├── README.md
└── visualizations/
    ├── survival_vs_sex.png
    ├── survival_vs_pclass.png
    ├── survival_count.png
    ├── fare_distribution_by_pclass.png
    ├── age_distribution.png
    ├── age_distribution_by_survival_boxplot.png
    └── age_distribution_by_survival.png
```

---

## Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Installation

Clone the repository:

```bash
git clone https://github.com/<your-username>/Titanic-Survival-Analysis.git
```

Move into the project directory:

```bash
cd Titanic-Survival-Analysis
```

Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn notebook
```

---

## Running the Project

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```
Titanic_Analysis.ipynb
```

Run all the cells sequentially.

---

## Data Preprocessing

The following preprocessing steps were performed:

- Loaded the dataset using Pandas.
- Explored the dataset using:
  - `head()`
  - `info()`
  - `describe()`
  - `shape`
- Checked and removed duplicate records.
- Filled missing values:
  - Age → Median
  - Embarked → Mode
- Dropped the Cabin column due to excessive missing values.
- Converted the Sex column into numerical values.
- Applied one-hot encoding on the Embarked column.
- Created a new feature named **FamilySize**.
- Removed unnecessary columns:
  - PassengerId
  - Name
  - Ticket
- Saved the processed dataset as:

```
Titanic_processed.csv
```

---

## Exploratory Data Analysis (EDA)

The following visualizations were generated:

- Survival Count Plot
- Gender vs Survival Count Plot
- Passenger Class vs Survival Plot
- Age Distribution Histogram
- Fare Box Plot
- Correlation Heatmap

---

## Key Observations

- Around 62% passengers died.
- Female passengers had a significantly higher survival rate than male passengers.
- First-class passengers had better survival chances than passengers in second and third class.
- The Age distribution showed that most passengers were young to middle-aged adults.
- The Fare column contained several high-value outliers, representing passengers who paid significantly higher fares.


---

## Output Files

This project generates the following files:

- `Titanic_survival_analysis.ipynb`
- `Titanic_revised.csv`
- `Report.docx`
- Visualization images

---

## Future Improvements

- Train machine learning models to predict passenger survival.
- Compare different classification algorithms.
- Perform hyperparameter tuning.
- Improve feature engineering.

---

## Conclusion

The Titanic dataset was successfully cleaned, transformed, and analyzed. Missing values were handled appropriately, categorical variables were encoded, and a new feature (**FamilySize**) was created. Exploratory Data Analysis revealed that gender, passenger class, and fare were among the most influential factors affecting passenger survival. The processed dataset is suitable for use in machine learning applications.

---

## Author

**Name:** Shabd Rastogi

**College:** Ajay Kumar Garg Engineering College (AKGEC)

**Domain:** Machine Learning

**Project:** Titanic Survival Analysis

---

## License

This project is submitted solely for educational purposes as part of the **BRL AKGEC Wildcard Task**.
