# 🛍️ Online Retail II Dataset - Exploratory Data Analysis (EDA)

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Status](https://img.shields.io/badge/Status-Complete-success.svg)
![CodeAlpha](https://img.shields.io/badge/CodeAlpha-Internship-orange.svg)

**CodeAlpha Data Analytics Internship - Task 2: Exploratory Data Analysis**

---

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Data Cleaning Steps](#Data-Cleaning-Steps)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Key Insights](#key-insights)
- [Recommendations](#Recommendations)
- [Challenges & Solutions](#challenges--solutions)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [Contact](#contact)

---

## 🎯 Overview

This project performs a complete **Exploratory Data Analysis (EDA)** on the **Online Retail II Dataset**, a real-world e-commerce dataset containing transactions from a UK-based online retail store (2009–2011).

### What This Project Does

1. Cleans messy retail transaction data
2.  Handles missing values, negative entries & duplicates
3. Generates descriptive statistics and visualizations
4. Performs univariate, bivariate & multivariate analysis
5. Conducts hypothesis testing (UK vs Non-UK sales)
6. Detects outliers using IQR
7. Extracts actionable **business insights**

A cleaned dataset is also included for reuse.
  

---

## ✨ Features

### 🧹 Data Cleaning
- Missing value handling
- Duplicate removal
- Negative & zero quantity/price filtering
- Data type corrections
- New feature creation: **TotalAmount, Year, Month, Day**

### 📊 Exploratory Data Analysis
- Distribution understanding
- Country-wise sales analysis
- Product performance comparison
- Monthly and weekly sales trends
- Heatmaps, scatter plots, bar charts

### 📈 Statistical Insights
- **T-test** comparing UK vs Non-UK transaction values
- Outlier identification using **IQR**
- Correlation matrix (Quantity, Price, TotalSales)

---

## 💻 Technologies Used

| Technology | Purpose |
|-----------|---------|
| **Python 3.8+** | Core programming language |
| **Pandas** | Data manipulation |
| **NumPy** | Numerical operations |
| **Matplotlib** | Data visualization |
| **Seaborn** | Advanced visual analytics |
| **SciPy** | Hypothesis testing |
| **Jupyter Notebook** | Interactive development environment |

---

## 🚀 Installation

### Prerequisites

- Python 3.8 or higher
- pip (Python package manager)
- Jupyter Notebook

### Step 1: Clone the Repository
```bash
git clone https://github.com/simitha2002/CodeAlpha_OnlineRetail_Analysis.git
cd CodeAlpha_OnlineRetail_Analysis
```

### Step 2: Create Virtual Environment (Recommended)
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Mac/Linux
python3 -m venv venv
source venv/bin/activate
```

## 📖 Usage

### Option 1: Run Jupyter Notebook
```bash
jupyter notebook notebooks/online_retail_EDA.ipynb
```

Then run all cells sequentially (Cell → Run All)

### Option 2: Quick Start
```python
# Import required libraries
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt

# Load cleaned data
df = pd.read_csv('data/online_retail_cleaned.csv')

df.head()
df.describe()
```

## 📁 Project Structure
---

```
CodeAlpha_OnlineRetail_Analysis_EDA/
│
├── Task 2.ipynb              # Main analysis notebook                  
│
├── data/
│   ├── online_retail_II.csv          # Original dataset (uncleaned)
│   └── Online_Retail_II_Cleaned.csv  # Cleaned dataset
│
└── README.md                               # Documentation
```

---

## 🧹 Data Cleaning Steps

- Removed missing **Customer ID** values
- Filled missing product **descriptions**
- Removed duplicates
- Removed negative quantities & prices
- Created new feature: `TotalSales = Quantity * Price`
- Converted invoice dates to datetime
- Extracted **Year, Month, Day**

---

## 🔎 Exploratory Data Analysis
**Includes:**
- **Univariate Analysis** (Price distribution)
- **Bivariate Analysis** (Quantity vs TotalSales, Country vs Sales)
- **Multivariate Analysis** (Monthly trends by year & country)
- **Correlation Analysis** (Price, TotalSales, Quantity)
- **Hypothesis Testing** (UK vs Non-UK transaction values)
- **Outlier Detection** using IQR

---

## 🔍 Key Insights

### 🌍 Market Insights

- The **United Kingdom** accounts for the vast majority of sales revenue.
- Other countries (Netherlands, Germany, France) show emerging potential.
  
### 📅 Seasonal Trends

- **November** is the highest sales month.
- **February** consistently shows lower sales.
- Weekdays outperform weekends significantly.

### 💰 Product Insights

- Top-selling products are **low-cost decorative items** (T-light holders, ornaments, craft products).
- Revenue is strongly driven by **quantity sold**, not price.

### 📈 Customer Behavior

- Many high-value transactions are **bulk or wholesale orders**, not errors.
- The dataset contains meaningful outliers that significantly influence revenue.
  
---

## 💡 Recommendations
- Focus marketing efforts on the **UK region.**
- Expand strategically into **Germany, Netherlands, France.**
- Maintain higher inventory during **October–November.**
- Introduce **volume discounts** for bulk buyers.
- Promote bundles of fast-moving decorative products.
- Investigate weekend sales gaps to improve engagement.
- Retain outlier records (they represent real revenue spikes).

---

## 🚧 Challenges & Solutions

### Challenge 1: Large number of missing Customer IDs 
**Solution:** Removed rows with missing unique identifiers (critical for analysis)  

### Challenge 2: Negative quantities and prices 
**Solution:** Filtered and validated all transactional data 

### Challenge 3: Highly skewed distributions  
**Solution:** Used log scaling and IQR-based outlier detection  

### Challenge 4: Many extreme outliers
**Solution:** reated them as **meaningful business events**, not errors

---

## 🔮 Future Enhancements

- [ ] Customer segmentation using **RFM Analysis**
- [ ] Build interactive dashboard (Tableau/Power BI)
- [ ] Forecast monthly sales using time-series models
- [ ] Product recommendation engine
- [ ] Automated reporting pipeline

---

## 🎓 Learning Outcomes

Through this project, I gained experience in:

- Real-world data cleaning  
- Exploratory analysis techniques  
- Visualization best practices 
- Statistical hypothesis testing
- Business story-telling from data
- Git & GitHub documentation
- Professional analytics workflow 

---

## 🤝 Contributing

Contributions are welcome!
1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch 
5. Open a Pull Request

---

## 📞 Contact

**Simitha Ummer**

- LinkedIn: [linkedin.com/in/simitha-ummer](http://www.linkedin.com/in/simitha-ummer-69a848350)
- GitHub: [github.com/simitha2002](https://github.com/simitha2002)
- Email: simithau@gmail.com

**Project Link:** [https://github.com/simitha2002/CodeAlpha_OnlineRetail_Analysis_EDA](https://github.com/simitha2002/CodeAlpha_OnlineRetail_Analysis_EDA)

---

## 🙏 Acknowledgments

- **CodeAlpha** for the internship opportunity
- **UCI & Kaggle** for publicly available data
- **Python Community** for powerful open-source tools

---

## ⭐ Show Your Support

If you found this project helpful, please give it a ⭐️!

---
