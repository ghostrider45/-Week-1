## Crop and Fertilizer Recommendation System using Machine Learning

This project involves creating a recommendation system for crops and fertilizers based on environmental factors using Machine Learning (ML). The dataset contains various features like nitrogen, phosphorus, potassium levels in the soil, temperature, humidity, pH, and rainfall. The goal is to analyze the dataset and prepare it for building an ML model.

**Project Structure**

1. **Prerequisites**

Before running the project, make sure to install the required Python libraries:

```bash
pip install opencv-python pandas numpy matplotlib seaborn
Dataset
The dataset used for this project is Crop_recommendation.csv. It contains the following columns:

N: Nitrogen content in soil
P: Phosphorus content in soil
K: Potassium content in soil
temperature: Temperature in degrees Celsius
humidity: Relative humidity in percentage
ph: pH value of the soil
rainfall: Rainfall in mm
label: Recommended crop
Steps Performed
Data Loading

The dataset is loaded using Pandas:

Python

import pandas as pd
crop = pd.read_csv("./dataset/Crop_recommendation.csv")
Exploratory Data Analysis (EDA)

Display the first and last rows of the dataset:
Python

crop.head()
crop.tail()
Check the shape of the dataset:
Python

crop.shape
Inspect data types and non-null counts:
Python

crop.info()
Check for missing and duplicate values:
Python

crop.isnull().sum()
crop.duplicated().sum()
Generate descriptive statistics:
Python

crop.describe()
Analyze class distribution for the label column:
Python

crop['label'].value_counts()
Visualization

The project leverages Matplotlib and Seaborn for data visualization (to be expanded in future updates). Examples include:

Visualizing distributions of soil nutrients.
Plotting relationships between environmental factors.
Key Findings
The dataset is clean with no missing or duplicate values.
The label column contains multiple crop types with varying frequencies.
The feature columns (N, P, K, temperature, etc.) have numeric data suitable for ML modeling.
Next Steps
Perform feature engineering and scaling.
Split the data into training and testing sets.
Train ML models (e.g., Random Forest, Decision Trees) for crop and fertilizer prediction.
Evaluate the model's performance using appropriate metrics.
How to Use

Clone this repository:
Bash

git clone [https://github.com/ghostrider45/-Week-1.git]
Install dependencies:
Bash
pip install -r requirements.txt

Run the Jupyter Notebook to explore the dataset and implement ML models.

