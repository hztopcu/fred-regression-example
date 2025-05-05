# 🚀 FRED Regression Example

A minimal Python script to:

* Fetch **FEDFUNDS** and **CPIAUCSL** data from the FRED API
* Perform a linear regression: `CPI ~ FEDFUNDS`
* Save results and visualize the trend line

---

## 🔧 Setup

1. **Python** 3.10 or newer
2. **Install dependencies**:

   ```bash
   pip install --upgrade pip
   pip install pandas pandas_datareader statsmodels matplotlib
   ```
3. **Configure your FRED API Key**:

   * **Windows CMD**:

     ```bat
     set FRED_API_KEY=YOUR_KEY
     ```
   * **PowerShell**:

     ```powershell
     $Env:FRED_API_KEY="YOUR_KEY"
     ```

---

## ▶️ Usage

Clone the repo and run:

```bash
python fred_regression_example.py
```

---

## 🗂️ Outputs

| File                     | Description                        |
| :----------------------- | :--------------------------------- |
| `regression_summary.txt` | Detailed regression summary output |
| `cpi_vs_fedfunds.png`    | Scatter plot with regression line  |

---

## 📈 Quick Interpretation

> **Regression Results**
>
> * **Dependent:** CPI (Consumer Price Index)
> * **Independent:** FEDFUNDS (Effective Federal Funds Rate)
> * **R²:** \~0.002 → explains only 0.2% of CPI variation
> * **Coefficient:** \~-0.15 (p > 0.05) → not statistically significant
> * **Intercept:** \~230 (p < 0.001)
> * **Conclusion:** Limited direct linear impact; other macro factors likely drive CPI changes

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1pxPI1egfDj0O41qAx0nM8LPjG9vDELSt?usp=sharing)

