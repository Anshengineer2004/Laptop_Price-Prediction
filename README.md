# 💻 Laptop Price - Exploratory Data Analysis (EDA)

This repository contains a comprehensive **Exploratory Data Analysis (EDA)** and data preprocessing notebook on a laptop pricing dataset. The project focuses on cleaning, visualizing, and analyzing how various technical specifications (like Processor Speed, RAM, Storage, etc.) influence the retail price of laptops.

---

## 📊 Dataset Overview
The dataset (`Laptop_price.csv`) contains **1,000 entries** with the following features:
* **Brand**: Laptop manufacturer (Asus, Acer, Lenovo, HP, Dell, etc.)
* **Processor_Speed**: Speed of the processor (in GHz)
* **RAM_Size**: Random Access Memory size (4GB, 8GB, 16GB, 32GB)
* **Storage_Capacity**: Internal storage (256GB, 512GB, 1000GB)
* **Screen_Size**: Size of the screen (in inches)
* **Weight**: Weight of the laptop (in kg)
* **Price**: Target variable (retail price of the laptop)

---

## 🛠️ Key Features of the Analysis
The analysis is structured into clear data science workflows:

1. **Data Loading & Inspection**: 
   * Initial checks using `.head()`, `.tail()`, `.info()`, and `.describe()`.
   * Verifying data types and missing values.
2. **Data Cleaning**:
   * Checking for null values (`isnull().sum()`) and duplicate entries (`duplicated().sum()`).
3. **Data Preprocessing**:
   * Encoding categorical features using one-hot encoding (`pd.get_dummies()`) to make the data ready for machine learning models.
4. **Data Visualization**:
   * Plotting price distribution histograms with Kernel Density Estimates (KDE) using `Seaborn` to understand market pricing trends.

---

## 🚀 Getting Started

### Prerequisites
Make sure you have the following Python libraries installed:
```bash
pip install pandas numpy matplotlib seaborn
