# 🚕 Sweet Lift Taxi Demand Forecasting
Forecast the number of taxi orders for the next hour to help Sweet Lift Taxi company optimize drive allocation and reduce wait times during peak hours. 

## 📖 Table of Contents
  - Project Description
  - Problem Statement
  - Features
  - Tools and Libraries Used
  - How to run this project locally
  - Usage
  - Results
  - Conclusion
  - Credits

## 📝 Project Description
The project aims to build a predictive model to forecast hourly taxi demand at airports using data provided by Sweet Lift Taxi. By accurately forecasting taxi orders, the company can ensure adequate driver availability during busy periods and improve customer satisfaction. 

## ❓ Problem Statement
Predict the number of taxi orders for the next hour using hourly data. The model should achieve an RMSE (Root Mean Squared Error) of no more than 48 on the test set.

## ✨ Features
  - Time series resampling and visualization
  - Evaluation of classical time series models (AR, MA, ARMA)
  - Benchmarking with machine learning models (Linear Regression, CatBoost, LightGBM, Random Forest)
  - Hyperparameter tuning and performance comparison
  - Final model deployment recommendation

## 🛠️ Tools and Libraries Used
  - Python 3
  - Pandas
  - NumPy
  - Matplotlib / Seaborn
  - Scikit-learn
  - CatBoost
  - LightGBM
  - Statsmodels

## 💻 How to run this project locally
  1. Clone the repository:
      ```bash
      git clone https://github.com/yourusername/sweet-lift-taxi-demand-forecasting.git
      cd sweet-lift-taxi-demand-forecasting
  2. Set up a virtual environment:
     ```bash
     python -m venv venv
     source venv/bin/activate  # On Windows use `venv\Scripts\activate`
  3. Install dependencies:
     ```bash
     pip install -r requirements.txt
  4. Run the notebook or script:
     ```bash
     jupyter notebook.ipynb

## 🧪 Usage
  1. Place the dataset in the /datasets/taxi.csv file path.
  2. Run the notebook or Python script to:
       - Load and resample the data
       - Analyze trends and seasonality
       - Train and evaluate models
  3. Get forecasts for future hourly taxi demand.

## 📊 Results
Model Performance (RMSE on test set):
| Model               | RMSE                |
| ------------------- | ------------------- |
| Moving Average      | 84.64               |
| AR (Autoregression) | 48.34               |
| ARMA                | 49.74               |
| Linear Regression   | \~80+ (Overfitting) |
| CatBoost            | \~45.7              |
| LightGBM            | \~44.5              |
| **Random Forest**   | **43.87**           |

  - Random Forest was selected as the final model due to its:
      - Lowest RMSE on the test set
      - Minimal overfitting
      - Strong generalization capabilities

## 📌 Conclusion
The project demonstrates the successful development of a reliable time series forecasting system for predicting hourly taxi demand at airports. While time series models offered reasonable performance, machine learning models—especially Random Forest—proved significantly more effective.
Sweet Lift Taxi can now deploy the Random Forest model to anticipate demand and allocate drivers proactively, thereby improving service efficiency and customer experience.

allocate drivers proactively, thereby improving service efficiency and customer experience.

## 🤝 Credits
This project was created as part of the TripleTen Data Science program. Special thanks to:
  - TripleTen instructors and peers for ongoing support and feedback.
  - Dataset provided by Sweet Lift Taxi (via simulated project prompt).

## 🛡️ License
This project is licensed under the MIT License.
