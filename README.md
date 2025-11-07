# Airline Passenger Demand Forecasting

## Project Overview
This project focuses on forecasting airline passenger demand using time series analysis.  
The objective is to analyze historical flight data, identify temporal patterns such as trends and seasonality, and develop a predictive model capable of forecasting future passenger volumes.  
Accurate forecasting supports improved flight scheduling, ticket pricing, and resource allocation within the aviation industry.

---

## Dataset
The dataset used in this project contains synthetic flight records covering the years 2023 to 2025.  
Each record represents an individual passenger and includes various features such as:

- Departure and arrival airports  
- Airline and flight details  
- Ticket price and delay time  
- Travel purpose and seat class  
- Passenger satisfaction score  

The key column for time series forecasting is `Departure_Time`, which was converted to a datetime format and aggregated by month to analyze passenger demand trends.

---

## Methodology
The project was developed in a Jupyter Notebook titled **Airline_forecasting.ipynb**.  
The following steps were carried out:

1. **Business Understanding**  
   Defined the forecasting goal and its importance in airline operations.

2. **Data Understanding**  
   Explored dataset structure, data types, and time coverage.  
   Converted `Departure_Time` to datetime and extracted additional date features.

3. **Data Preparation**  
   Aggregated passenger counts on a monthly basis, handled missing values, and sorted the dataset chronologically.

4. **Exploratory Data Analysis (EDA)**  
   Visualized overall passenger demand trends, seasonal fluctuations, and compared airline-level performance.  
   Examined relationships between variables such as price, satisfaction, and delays.

5. **Modeling and Forecasting**  
   Applied an ARIMA model to forecast monthly passenger demand.  
   Evaluated performance using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).

6. **Forecast Visualization**  
   Generated a 12-month forecast displaying expected passenger demand patterns and seasonal peaks.

---

## Results and Findings
- Passenger demand displayed consistent seasonal fluctuations, with noticeable peaks during high-travel months.  
- The ARIMA model successfully captured both trend and seasonality in the time series data.  
- Forecasted results closely matched observed patterns, validating the model’s predictive accuracy.  
- The analysis demonstrated the practical use of statistical forecasting in airline capacity and pricing management.

---

## Technologies Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Statsmodels (ARIMA)  
- Scikit-learn  

---

## Files in This Repository
| File Name | Description |
|------------|-------------|
| **Airline_forecasting.ipynb** | Contains the full workflow for data preparation, analysis, and forecasting. |
| **synthetic_flight_passenger_data.csv** | Dataset containing flight and passenger information used for analysis. |
| **README.md** | Project summary and documentation. |

---

## Conclusion
The project demonstrated how time series forecasting can effectively predict airline passenger demand and support strategic decision-making.  
Future improvements may include the integration of external factors such as weather conditions or economic indicators, as well as the implementation of more advanced models such as SARIMA, Prophet, or LSTM to enhance forecasting accuracy.

