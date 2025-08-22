# Solar Panel Performance Monitoring & Prediction

### Project Goal
The aim of this project is to design and implement machine learning models for real-time solar panel performance monitoring and prediction. The focus is on:

* Estimating soiling rate and panel degradation
* Forecasting power output using weather and sensor data
* Optimizing cleaning schedules for maximum efficiency
* Providing string-level insights to support operational decision-making

---

### Data Description
Two main datasets are used in this project:

**Generation Data (`Plant_1_Generation_Data.csv`)**
Contains solar plant electricity generation records.
Key columns:
* `DATE_TIME`: Timestamp of the reading
* `DC_POWER`: Power generated at DC level
* `AC_POWER`: Power generated at AC level
* `DAILY_YIELD`: Daily energy yield
* `TOTAL_YIELD`: Cumulative energy yield

**Weather Sensor Data (`Plant_1_Weather_Sensor_Data.csv`)**
Captures environmental and operational conditions.
Key columns:
* `DATE_TIME`: Timestamp of the reading
* `AMBIENT_TEMPERATURE`: Temperature of the surrounding environment
* `MODULE_TEMPERATURE`: Temperature of the solar module
* `IRRADIATION`: Solar irradiance received

Both datasets are aligned on `DATE_TIME` and `PLANT_ID`, enabling integrated analysis.

---

### Project Stages
* **Data Preprocessing & Integration**
    * Cleaning and aligning generation + weather datasets.
    * Handling missing values and resampling for consistency.
* **Exploratory Data Analysis (EDA)**
    * Visualizing generation trends, temperature impact, and irradiation influence.
    * Identifying patterns of soiling and degradation.
* **Feature Engineering**
    * Extracting meaningful features from raw sensor data (efficiency, performance ratio, temporal features).
    * Incorporating external data sources (IMD forecasts, geospatial layers, etc.).
* **Model Development**
    * Building predictive models (CNN, XGBoost) for power output forecasting.
    * Evaluating model performance on real-time and historical data.
* **Analytics Pipeline**
    * Computing panel efficiency and performance ratios.
    * Generating string-level operational insights.
    * Suggesting optimized cleaning schedules.
* **Deployment & Monitoring (Future Work)**
    * Real-time dashboards for solar asset operators.
    * Automated alerts for efficiency drop or abnormal patterns.

---

This project demonstrates how multi-source data and machine learning can transform solar plant operations by enabling predictive maintenance, smarter scheduling, and higher efficiency. It not only strengthens reliability but also maximizes returns from renewable energy investments.
