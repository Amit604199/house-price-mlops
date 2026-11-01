# House Price Prediction Using MLOps

## 1. Project Overview
This project predicts house prices using Machine Learning and MLOps concepts. It uses Linear Regression to estimate house prices based on property features such as area, bedrooms, bathrooms, and house age.

## 2. Project Objectives
- Predict house prices using Machine Learning.
- Train and evaluate a Linear Regression model.
- Track experiments using MLflow.
- Save the trained model using Joblib.
- Deploy the model using FastAPI.

## 3. Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- MLflow
- FastAPI
- Joblib
- Uvicorn

## 4. Machine Learning Algorithm
**Linear Regression**

The model uses the following input features:
- Area (sqft)
- Number of Bedrooms
- Number of Bathrooms
- House Age

Output: Predicted House Price.

## 5. Project Structure

```text
amit-house-price-mlops/
│
├── data/
│   └── house_prices.csv
├── models/
│   └── house_model.joblib
├── api.py
├── generate_data.py
├── train.py
├── requirements.txt
└── .gitignore
```

## 6. Installation and Setup

Clone the repository:

```bash
git clone https://github.com/Amit604199/house-price-mlops.git
```

Go to the project folder:

```bash
cd house-price-mlops
```

Install dependencies:

```bash
pip install -r requirements.txt
```

## 7. Generate Dataset

```bash
python generate_data.py
```

## 8. Train the Model

```bash
python train.py
```

The trained model is saved in the models folder.

## 9. Run the FastAPI Application

```bash
uvicorn api:app --reload
```

Open the API documentation:

http://127.0.0.1:8000/docs

Use the `/predict` endpoint to predict house prices.

## 10. MLflow Experiment Tracking

Run MLflow UI:

```bash
mlflow ui --host 127.0.0.1 --port 5000 --workers 1
```

Open:

http://127.0.0.1:5000

## 11. Model Evaluation
The model is evaluated using:
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

## 12. Dataset Information
This project uses a synthetically generated dataset containing house-related features and prices. Predictions are for educational demonstration and should not be treated as actual market valuations.

## 13. Author
**Amit**

## 14. Conclusion
This project demonstrates a basic end-to-end Machine Learning workflow, including dataset generation, model training, experiment tracking, model saving, and API deployment.
