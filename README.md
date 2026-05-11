# Precision_Farming
A data analytics project optimizing crop management using Python. Analyzes soil nutrients (N, P, K) and climatic factors (temperature, rainfall) to recommend suitable crops for specific conditions. Features extensive EDA and visualization to aid precision farming decisions.
# Precision Farming: Leveraging Data Analytics & Prediction for Enhanced Crop Management

## 📌 Project Overview
Precision Farming is a data-driven approach to agriculture that optimizes crop yield by analyzing environmental and soil conditions. This project leverages Exploratory Data Analysis (EDA) to recommend the most suitable crops based on specific soil and climatic parameters. The goal is to assist farmers and agricultural professionals in making informed decisions to maximize productivity and sustainability.

## 📂 Dataset
The dataset consists of 2,200 records with the following parameters:

* Nitrogen (N): Ratio of Nitrogen content in soil.
* Phosphorus (P): Ratio of Phosphorous content in soil.
* Potassium (K): Ratio of Potassium content in soil.
* Temperature: Temperature in degree Celsius.
* Humidity: Relative humidity in %.
* pH: pH value of the soil.
* Rainfall: Rainfall in mm.
* Label (Target): The recommended crop (22 unique crops including Rice, Maize, Coffee, etc.).

Source: Kaggle - Crop Recommendation Dataset](https://www.kaggle.com/datasets/atharvaingle/crop-recommendation-dataset).

## 🛠️ Tech Stack & Prerequisites
The analysis was performed using Python and the following libraries:

1. Language: Python
2. Libraries: Pandas, NumPy, Scikit-Learn, Seaborn, Matplotlib, Plotly, Ipywidgets.
   * Pandas & NumPy: Data manipulation and preprocessing.
   * Matplotlib & Seaborn: Static data visualization (Histograms, Heatmaps, Boxplots).
   * Ipywidgets: Interactive analysis (Dropdowns for crop-specific stats).
   * SciPy: Statistical analysis (Pearson correlation).
3. Platform: Jupyter Notebook
   * Jupyter Notebook: Interactive development environment.
4. IBM SPSS Statistics

## 📊 Methodology & Key Analysis
The project follows a structured data analytics & prediction lifecycle:

1.  Data Pre-processing: Checked for missing values and duplicates (none found).
2.  Descriptive Statistics: Analyzed mean, min, max, and quartiles for all variables.
3.  Skewness & Kurtosis: Assessed data distribution; found Rainfall to be moderately skewed and Potassium to be leptokurtic.
4.  Correlation Analysis: Used Pearson's correlation to find relationships, such as the link between Rainfall and soil pH.
5.  Visualization:
    * Histograms & Density Plots: To view distribution of soil nutrients.
    * Box Plots: To identify outliers in temperature and rainfall.
    * Pair Plots: To observe pairwise relationships between variables.
6. Predictive Modeling: Implementation of multiple ML algorithms including:
    * Random Forest
    * Decision Trees
    * K-Nearest Neighbors (KNN)
    * Logistic Regression
    * Naive Bayes
7.  Irrigation Calculator: A custom tool that calculates the water deficit based on current rainfall and the optimal needs of the selected crop, providing exact irrigation requirements in liters based on land area.

## 🌾 Key Findings
* Nitrogen Requirements: Cotton requires very high Nitrogen, while crops like Kidney Beans and Lentils require low Nitrogen.
* Phosphorus & Potassium: Grapes and Apples have high P and K requirements.
* Rainfall Dependency: Rice, Papaya, and Coconut are identified as high-rainfall (Monsoon) crops.
* Seasonal Recommendations:
    * Summer Crops: Pigeonpeas, Mothbeans, Blackgram.
    * Winter Crops: Maize, Lentil, Pomegranate.
* Soil pH: Most crops prefer slightly acidic to neutral soil (pH 6–7.5).

## 📈 Results
The models were evaluated based on accuracy, precision, and recall. The **Random Forest** and **Naive Bayes** models typically demonstrate high performance in recommending crops accurately based on the soil-climate profile.
