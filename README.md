#  🌦 Weather Forecasting

A data-driven weather forecasting project using Prophet and visualizations in Python.

#  Weather forecasting in Delhi using Python & Prophet
This project is a time series forecasting model that analyzes and predicts the mean daily temperature in Delhi using historical weather data. It includes visualizations and forecasting using **Facebook Prophet**, a powerful time series prediction library.

---

## 📁 Dataset

The dataset used: `DailyDelhiClimateTrain.csv`

- 📆 Date range: 2013 to 2017
  
- 📌 Columns:
  - `date`: Date of record
  - `meantemp`: Mean temperature
  - `humidity`: Humidity levels
  - `wind_speed`: Wind speed
  - `meanpressure`: Atmospheric pressure

---

## 📊 Visualizations

- 📈 Line plots of temperature, humidity, wind speed over time
- 🌡 Scatter plot of temperature vs. humidity with trendline
- 📅 Year-wise temperature trends (monthly breakdown using seaborn)
- 🔮 Future temperature forecast using **Prophet**

---

## 🔮 Forecasting

We used [Prophet](https://facebook.github.io/prophet/) for temperature prediction:


from prophet import Prophet

model = Prophet()

model.fit(forecast_data)

future = model.make_future_dataframe(periods=365)

forecast = model.predict(future)


✅ The model predicts temperature trends up to 1 year into the future.

---

💻 Technologies Used

Python

Pandas

NumPy

Plotly

Seaborn

Matplotlib

Prophet (by Facebook)

---

🚀 How to Run

1.Clone this repo or download the notebook.

2.Open weather_forecast_delhi.ipynb in Google Colab or Jupyter Notebook.

3.Install dependencies (in Colab, you can run the following cell):

!pip install prophet plotly seaborn

4.Run all cells to visualize and forecast temperature trends.

---

📌  Graphs

<img width="1240" height="510" alt="image" src="https://github.com/user-attachments/assets/7910cf18-8385-4642-bf15-933b26d37bc8" />
<img width="1256" height="531" alt="image" src="https://github.com/user-attachments/assets/0908aace-6fa1-4af3-8ca0-09b1669ef8ad" />
<img width="1242" height="520" alt="image" src="https://github.com/user-attachments/assets/a6296961-fc87-473a-a1e0-920d72c7fe5c" />
<img width="1246" height="529" alt="image" src="https://github.com/user-attachments/assets/36d70962-c580-476b-98d2-8daf93a2176c" />
<img width="1248" height="553" alt="image" src="https://github.com/user-attachments/assets/a2929159-8317-41fd-bff6-ed58038da7cc" />
<img width="892" height="552" alt="image" src="https://github.com/user-attachments/assets/d570a6d2-86d5-4eb5-b337-37ec3014d297" />





---


📚 References

Dataset: Kaggle - Daily Climate Data of Delhi

---

🧑‍💻 Author

Sharvika Rajiyahan



