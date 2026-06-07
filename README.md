# Weather Trend Forecasting

## PM Accelerator Mission

By making industry-leading tools and education available to individuals from all backgrounds, PM Accelerator helps level the playing field for future professionals in Product Management, Data Science, Artificial Intelligence, and Technology. Through mentorship, networking, and project-based learning, PM Accelerator provides opportunities for individuals to gain practical experience and develop industry-relevant skills.

---

## Project Overview

This project analyzes the Global Weather Repository dataset to identify weather trends, explore environmental patterns, and forecast future temperature behavior using machine learning and time-series forecasting techniques.

The analysis includes:

* Data Cleaning & Preprocessing
* Exploratory Data Analysis (EDA)
* Anomaly Detection
* Climate Analysis
* Environmental Impact Analysis
* Feature Importance Analysis
* Spatial & Geographical Analysis
* Weather Forecasting using Multiple Models

---

## Dataset

**Dataset:** Global Weather Repository

**Source:** Kaggle

https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository

The dataset contains daily weather observations from locations worldwide, including:

* Temperature
* Humidity
* Wind Speed
* Atmospheric Pressure
* Precipitation
* UV Index
* Cloud Coverage
* Air Quality Indicators (PM2.5, PM10)
* Latitude & Longitude
* Weather Conditions

---

## Data Cleaning & Preprocessing

The following preprocessing steps were performed:

* Checked and handled missing values
* Removed duplicate records
* Converted `last_updated` to datetime format
* Created time-based features (Year, Month, Day)
* Detected outliers using the IQR method
* Standardized numerical features using StandardScaler

---

## Exploratory Data Analysis (EDA)

The following analyses were conducted:

* Temperature Distribution Analysis
* Precipitation Distribution Analysis
* Temperature vs Humidity Analysis
* Correlation Analysis
* Weather Trend Visualization

### Key Findings

* Most temperature observations fall within moderate ranges.
* Precipitation data is highly skewed, with many low-rainfall observations.
* Humidity shows a strong relationship with temperature.
* Pressure, cloud coverage, and wind speed exhibit meaningful correlations with temperature.

---

## Advanced Analysis

### Anomaly Detection

Implemented **Isolation Forest** to identify unusual weather observations and potential extreme weather events.

### Climate Analysis

Analyzed temperature trends across countries and seasons to understand long-term climate patterns.

### Environmental Impact Analysis

Examined relationships between weather variables and air quality indicators such as PM2.5 and PM10.

### Feature Importance Analysis

Used **Random Forest Regressor** to identify the most influential variables affecting temperature prediction.

Top contributing features included:

* Humidity
* Atmospheric Pressure
* UV Index
* Cloud Coverage

### Spatial & Geographical Analysis

Visualized weather patterns using latitude and longitude data to compare climate conditions across different regions and countries.

---

## Forecasting Models

The `last_updated` feature was used for time-series forecasting.

Models implemented:

* ARIMA
* Random Forest Regressor
* Ensemble Model

### Evaluation Metrics

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

| Model         | MAE   | RMSE  | R² Score |
| ------------- | ----- | ----- | -------- |
| ARIMA         | 1.470 | 2.290 | -0.229   |
| Random Forest | 0.384 | 1.211 | 0.658    |
| Ensemble      | 0.853 | 1.554 | 0.437    |

### Best Performing Model

**Random Forest Regressor**

The Random Forest model achieved the lowest MAE and RMSE while producing the highest R² score, making it the strongest forecasting model in this project.

---

## Key Insights

* Humidity is one of the strongest predictors of temperature.
* Air quality indicators show measurable relationships with weather conditions.
* Weather characteristics vary significantly across geographic regions.
* Locations closer to the equator generally experience higher temperatures.
* Machine learning models outperformed traditional statistical forecasting methods on this dataset.

---

## Repository Structure

```text
├── PM_Accelerator.ipynb
├── Weather_Trend_Forecasting_Report.pdf
├── README.md
├── requirements.txt
└── Global_Weather_Repository.csv
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/weather-trend-forecasting.git
cd weather-trend-forecasting
```

Install required packages:

```bash
pip install -r requirements.txt
```

---

## Running the Project

1. Open `PM_Accelerator.ipynb` using Jupyter Notebook or Google Colab.
2. Load the Global Weather Repository dataset.
3. Run all notebook cells sequentially.
4. Review the generated visualizations, analyses, and forecasting results.


---

## Conclusion

This project demonstrates the application of data science and machine learning techniques for weather trend analysis and forecasting. Through data preprocessing, exploratory analysis, anomaly detection, environmental studies, geographical pattern analysis, and predictive modeling, valuable insights were extracted from global weather data while achieving accurate temperature forecasting results.
