This repository contains two main data analysis (Capstone) projects developed in Python, focused on distinct areas: Stock Market Analysis and Emergency Calls (911) Analysis.

Below is a README.md template you can use in your GitHub repository.

# 📊 Data Science Capstone Projects

This repository brings together practical data science projects exploring exploratory data analysis (EDA), data visualization, and financial concepts.

---

## 📂 Included Projects

### 1. 📈 Stock Portfolio Analysis  
**File:** `Stock-Analysis-Capstone-Project.ipynb`

This project focuses on extracting and analyzing historical financial asset data using the **yfinance** library.

**Objective:**  
Build a stock portfolio, analyze historical returns and volatility, and visualize asset performance over time.

**Main Activities:**
- Real-time data extraction via Yahoo Finance  
- Daily and cumulative return calculations  
- Risk vs. return analysis (Efficient Frontier)  
- Visualization of adjusted closing prices and asset correlations  

**Technologies:**  
Python, Pandas, Matplotlib, Seaborn, yfinance

---

### 2. 🚨 911 Emergency Calls Analysis  
**File:** `DataCapstone_Project.ipynb`

A detailed analysis of a Kaggle dataset containing emergency call records from Montgomery County, PA.

**Objective:**  
Identify temporal and geographic patterns in emergency calls to understand the main service demands (EMS, Fire, Traffic).

**Main Activities:**
- Data processing and cleaning (Feature Engineering with DateTime objects)  
- Identification of the most frequent call types  
- Temporal analysis (calls by day of week, month, and hour)  
- Basic geospatial visualization based on zip codes and townships  

**Technologies:**  
Python, Pandas, NumPy, Matplotlib, Seaborn

---

## 🛠️ Installation and Requirements

To run the notebooks locally, it is recommended to use Anaconda or a Python virtual environment.

### Clone the repository
```bash
git clone https://github.com/your-username/repository-name.git
```
Install dependencies
```bash
pip install pandas numpy matplotlib seaborn yfinance
```
Open Jupyter Notebook

📈 Results and Conclusions
Stocks:
The notebook demonstrates how risk and return vary across different sectors (Technology, Energy, Healthcare) and how diversification impacts portfolio performance.

911:
The analysis revealed that EMS (Emergency Medical Services) calls are the most common and that there are specific peak hours for traffic-related incidents during business hours.

✒️ Author
Felipe Gurgel Araujo

Note: This project was developed as part of an academic activity.
