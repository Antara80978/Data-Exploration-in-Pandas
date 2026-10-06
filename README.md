# Exploratory Data Analysis (EDA) with Pandas

This repository contains Python scripts demonstrating baseline **Exploratory Data Analysis (EDA)** using the Pandas library on two iconic machine learning datasets: **Iris** and **Titanic**. 

Each script highlights a different style of data exploration—handling clean, numerical features (Iris) versus diagnosing messy, real-world data (Titanic).

## 🚀 Getting Started

### Prerequisites
Make sure you have Python installed along with the required libraries. You can install the dependencies via pip:

```bash
pip install pandas seaborn
```

---

## 📊 Datasets Overview

### 1. Iris Flower Dataset (`iris_exploration.py`)
* **Goal**: Understand the physical patterns that distinguish three species of Iris flowers (*setosa, versicolor, virginica*).
* **Key Steps Demonstrated**:
  * Dimension checks and dataset shapes.
  * Checking for target class balance using `.value_counts()`.
  * Feature aggregation using `.groupby()` to see average measurements per species.
  * Feature interaction profiling using numerical `.corr()`.

### 2. Titanic Passenger Dataset (`titanic_exploration.py`)
* **Goal**: Analyze the demographics and passenger attributes to find out which groups had higher survival rates.
* **Key Steps Demonstrated**:
  * Head/Tail data previews for mixed data types (categorical and numerical).
  * Missing value identification using `.isnull().sum()`.
  * Normalizing value counts to get overall percentage distributions (Survival Rate).
  * Pivot-style analysis using `.groupby()` to evaluate survival across multiple variables like *Sex* and *Ticket Class*.
  * Scanning for duplicate entries.

---

## 🛠️ Code Structure & Usage

You can save the scripts to your local machine and run them directly in your terminal or inside an IDE (like VS Code or Jupyter Notebook).

### Running the Iris Exploration
```bash
python iris_exploration.py
```

### Running the Titanic Exploration
```bash
python titanic_exploration.py
```

---

## 💡 Key Takeaways from EDA
* **Iris**: Reveals a strong correlation between petal length and width. Clear statistical boundaries emerge when grouping data by species, proving it is highly separable.
* **Titanic**: Highlights significant missing data issues (especially in the `age` and `deck` columns) and reveals strong demographic survival biases (e.g., higher survival rates among female and 1st-class passengers).
