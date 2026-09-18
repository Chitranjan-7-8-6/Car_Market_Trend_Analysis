# 🚗 Car Market Trends Analysis — CarDekho Dataset

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-Numerical%20Computing-013243?logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-11557C)
![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-4C72B0)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

An exploratory data analysis project on real used-vehicle listings from **CarDekho**, built to answer 25 practical questions about pricing, depreciation, and "good deal" detection — covering both **cars and two-wheelers**.

---

## 📌 Project Info

| | |
|---|---|
| **Author** | Chitranjan Vishwakarma |
| **Course** | BCA (Bachelor of Computer Applications) |
| **College** | Sri Ram Kishun P.G. College, Gokul, Karsada, Varanasi |
| **AICTE Student ID** | STU6a6aca966acaf1785383574 |
| **Type** | VOIS DIY Project |

---

## 📖 About the Project

Anyone who has tried buying or selling a used car or bike knows the problem: it's genuinely hard to tell if the asking price is fair for the vehicle's age, mileage, and condition. This project digs into a real 301-listing CarDekho dataset to make those patterns visible.

The twist: the raw data mixes **cars and bikes together** under a single `Car_Name` column with no label telling them apart. So before any of the vehicle-specific questions could be answered, the dataset had to be split into `Car` / `Bike` categories from the model names themselves — one of the more interesting parts of this project.

From there, the notebook works through **25 structured questions**, covering everything from basic data profiling to brand-wise depreciation trends to a small regression model that flags vehicles which sold for more than expected.

---

## 🗂️ Dataset

**File:** `Car_Market_Trends_Analysis_with_Car_Dekho_Data.csv`

| Detail | Value |
|---|---|
| Records | 301 |
| Manufacturing years | 2003 – 2018 |
| Vehicle types | 200 Cars, 101 Bikes |
| Columns | `Car_Name`, `Year`, `Selling_Price`, `Present_Price`, `Kms_Driven`, `Fuel_Type`, `Seller_Type`, `Transmission`, `Owner` |
| Missing values | None (2 exact duplicate rows found) |

---

## ❓ Questions Answered

The notebook is organized around 25 questions grouped into four parts:

1. **Data Overview (Q1–Q11)** — year range, price range, record count, missing data, most-sold vehicle, CNG vehicles, individual sellers, automatic transmission, single-owner count
2. **Depreciation & Pricing Factors (Q12–Q16)** — most/least depreciated vehicles, brand-wise depreciation, what factors drive depreciation, whether age/mileage affect price, a look at post-2014 vehicles
3. **Two-Wheeler Deep Dive (Q17–Q21)** — oldest/newest/most-sold bike, and bikes that sold above expected market value
4. **Car Deep Dive (Q22–Q25)** — oldest/newest car, and cars that sold above expected market value

---

## 🛠️ Tech Stack

- **Python 3** — core language
- **pandas & NumPy** — data cleaning, feature engineering (Vehicle_Type, Age, Depreciation %)
- **Matplotlib & Seaborn** — all charts (bar plots, box plots, scatter plots, count plots)
- **NumPy linear regression (least squares)** — builds an "expected price" for each vehicle to spot deals that beat the general trend
- **Jupyter Notebook** — where the whole analysis was written and run

---

## 📁 Project Structure

```
Car-Market-Trends-Analysis/

│---index.html                         # Meaningful Insights in Dashboard
├── car_market_trends_analysis.ipynb   # Main analysis notebook (all 25 questions)
├── car_market_trends_analysis.pdf     # PDF export of the notebook
├── Car_Market_Trends_Analysis_with_Car_Dekho_Data.csv   # Source dataset
├── Car_Market_Trends_Analysis_PPT.pptx                   # Project presentation
└── README.md                          # You are here
```

---

## ▶️ How to Run

1. Make sure Python 3 is installed, along with the required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
2. Keep `car_market_trends_analysis.ipynb` and the CSV file in the **same folder**.
3. Launch Jupyter and run all cells:
   ```bash
   jupyter notebook car_market_trends_analysis.ipynb
   ```

---

## 💡 Key Insights

- **Price is driven mostly by present price and age** — older vehicles sell for less, but kilometers driven alone barely moves the needle in this dataset.
- **Royal Enfield and Hyundai** hold their resale value the best (lowest average depreciation %); **Toyota and Bajaj** depreciate the most.
- Roughly **half the listings** are from 2015 onward, and these newer vehicles command noticeably higher average prices.
- A handful of vehicles — a few premium bikes (Royal Enfield, KTM) and a very low-mileage Toyota Fortuner — sold for well above what a simple price-prediction model expected, pointing to brand strength and low usage as real value drivers.

---

## 🙌 Acknowledgements

Dataset sourced from **CarDekho** used-vehicle listings. Built as part of an VOIS DIY project assignment.

---

<p align="center"><i>⭐ If you found this analysis useful, feel free to star the repo!</i></p>
