
# Laptop Price Analysis

This project is a simple Jupyter Notebook that performs Exploratory Data Analysis (EDA) and data preprocessing on a laptop pricing dataset.

---

## About the Dataset
The dataset (`Laptop_price.csv`) contains information about different laptops and their retail prices:
* **Brand**: The brand of the laptop (Dell, HP, Lenovo, etc.)
* **Processor_Speed**: Clock speed of the processor in GHz.
* **RAM_Size**: Memory size (4GB, 8GB, 16GB, 32GB).
* **Storage_Capacity**: Storage space (256GB, 512GB, 1000GB).
* **Screen_Size**: Display size in inches.
* **Weight**: Weight of the laptop in kilograms.
* **Price**: The selling price of the laptop (Target Variable).

---

## What this Notebook does:

1. **Loads the Data**: Reads the dataset using Pandas and displays basic information.
2. **Cleans the Data**: Checks for missing (null) values and duplicate rows.
3. **Preprocesses the Data**: Converts the categorical "Brand" column into numbers using One-Hot Encoding (`pd.get_dummies()`).
4. **Visualizes the Data**: Plots simple graphs using Seaborn and Matplotlib to analyze relationships.

---

## 📊 Key Insights from Visualizations

Based on the plots generated in this notebook:

* **Price Distribution (Tri-modal)**: The laptop prices are not normally distributed. Instead, they fall into three distinct price tiers: budget (~10,000), mid-range (~17,000), and premium (~32,000).
* **Feature Correlation (Heatmap)**: **Storage Capacity** has a perfect linear correlation of `1.00` with the Price, making it the single most dominant factor determining the laptop's cost in this dataset. Other features like RAM and Processor Speed show almost no direct linear correlation with price on their own.
* **RAM vs Price (Scatter Plot)**: Laptops across all RAM sizes (4GB to 32GB) exist within the three specific price bands. This confirms that RAM size alone does not push a laptop into a higher price tier in this dataset.

---
