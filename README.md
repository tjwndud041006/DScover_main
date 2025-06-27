# Weather Forecast Error Correction

This project addresses the correction of forecast errors caused by the spatial difference between meteorological forecast grids and actual observation points. Accurate 24-hour ahead weather prediction is essential for efficient operation of energy facilities such as solar power plants and gas turbines.

---

## **Project Overview**

- **Objective**: Develop a machine learning model to correct forecast errors using historical data.
- **Key variables**: Temperature (°C), Humidity (%), Atmospheric Pressure (hPa)
- **Modeling period**: 2024.01.01 ~ 2025.03.31 (15 months)

---

## **Data Description**

### 1. Training Data
- **Frequency**: Hourly
- **Format**: CSV
- **Forecast Data**: Extracted from LDAPS grid point closest to the observation site
- **Observation Data**: Collected at the power generation facility location

### 2. Evaluation Data
- **Period**: 2025.07 (1 month)
- **Observation data**: Not provided during evaluation
- **Evaluation metrics**: MAE (Mean Absolute Error), RMSE (Root Mean Squared Error)

---

## **Sample Data Format**
**Forecast Data**

```csv
기상관측일시,일사량,습도(%),절대습도,기온(degC),대기압(hPa)
2024-01-01 10:00:00,196.56,53.61,0.004,4.01,1012.17
2024-01-01 11:00:00,323.78,49.06,0.004,6.42,1011.96


