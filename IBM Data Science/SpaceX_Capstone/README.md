# 🚀 SpaceX Falcon 9 First Stage Landing Prediction

This project was developed as the Capstone for the **IBM Data Science Professional Certificate**.  
The goal is to build a machine learning pipeline to **predict whether the first stage of a SpaceX Falcon 9 rocket will successfully land**, which plays a key role in reducing launch costs through reusability.

---

## 📌 Objective

- Collect and process real-world data from the SpaceX API and Wikipedia
- Perform data wrangling and feature engineering
- Explore insights using data visualization and SQL
- Build an interactive dashboard with Plotly Dash
- Train and evaluate multiple classification models to predict landing success

---

## 📂 Project Structure
|-- spacex-data-collection-api.ipynb         # Collected launch data using SpaceX REST API
|-- spacex-data-webscraping.ipynb            # Scraped Wikipedia for booster & landing outcome data
|-- spacex-Data wrangling.ipynb              # Cleaned, merged, and engineered features
├── eda_using_dataviz.ipynb                  # Performed visual EDA using Seaborn and Matplotlib
├── eda-using-sql.ipynb                      # SQL-based EDA with SQLite queries
├── spacex-launch_site_location.ipynb        # Mapped launch and landing sites using Folium
├── spacex-dash-app.py                       # Interactive dashboard using Plotly Dash
├── SpaceX_Machine Learning Prediction.ipynb # Trained and evaluated ML models (LogReg, SVM, DT, KNN)
└── README.md                                # You are here!


---

## 📡 Data Collection

- Pulled structured JSON data using the [SpaceX Launches API](https://api.spacexdata.com/v4/launches/query)
- Supplemented landing outcomes and booster information via **web scraping** from Wikipedia using `BeautifulSoup`

---

## 🧹 Data Wrangling & Feature Engineering

- Cleaned and standardized multiple sources
- Removed missing and duplicate records
- Engineered features like:
  - `Class` (1 = successful landing, 0 = failed)
  - Orbit category
  - Booster version
  - Payload mass range
- Final dataset merged using `flight_number` as the primary key

---

## 📊 Exploratory Data Analysis

- **Visual EDA**: Seaborn & Matplotlib to explore distributions, correlations, and trends
- **SQL-based EDA**: Ran SQLite queries to analyze launch success by site, orbit, and payload
- **Geo-EDA**: Used Folium to map launch and landing site coordinates

---

## 🧠 Machine Learning Models

Trained and evaluated the following classifiers:
- Logistic Regression  
- Support Vector Machine (SVC)  
- Decision Tree  
- K-Nearest Neighbors (KNN)

✅ Used **GridSearchCV** to tune hyperparameters  
✅ Evaluated using accuracy, precision, recall, and F1-score  
✅ Selected best-performing model based on test set metrics

---

## 📈 Interactive Dashboard (Plotly Dash)

Built a responsive dashboard that allows users to:
- Select launch sites from a dropdown
- Adjust payload range via slider
- View pie charts of success distribution
- Visualize correlation between payload and landing outcome



