# House Price Prediction Model

A machine learning project that predicts housing prices based on features like bedrooms, bathrooms, size, lot size, and location.

## Project Overview

This project implements a complete machine learning pipeline for real estate price prediction. It includes data preprocessing, 
feature engineering, model training and evaluation, and a web application for making predictions.

## Features

- **Data preprocessing**: Handling missing values and standardizing measurements
- **Feature engineering**: Creating derived features like price per square foot and bedroom-bathroom ratio
- **Multiple models**: Implementation of Ridge Regression, ElasticNet, and ensemble methods
- **Hyperparameter tuning**: Grid search for optimal model parameters
- **Feature importance analysis**: Understanding which features most influence housing prices
- **Web application**: User-friendly interface for making predictions
- **Deployment configuration**: Ready for cloud deployment

## Installation

Clone the repository and install the required packages:

```bash
git clone https://github.com/Wawira-Muthoni/House-Price-Prediction.git
cd House-Price-Prediction
pip install -r requirements.txt
```

## Dataset

The model is trained on housing data with the following features:
- Number of bedrooms
- Number of bathrooms
- House size (square feet)
- Lot size (square feet/acres)
- ZIP code
- Price (target variable)

Place your training and test datasets in the project root directory as `train.csv` and `test.csv`.

## Usage

### Model Training

To train the model and evaluate its performance:

```bash
python train_model.py
```

This will:
1. Load and preprocess the data
2. Create and select features
3. Train multiple models
4. Compare model performance
5. Save the best model for later use

### Making Predictions

Run the Flask application:

```bash
python app.py
```

Then open your browser to `http://localhost:5000` to access the prediction interface.

## Model Performance

The final model achieved:
- RMSE (Root Mean Squared Error): [Add your value]
- R² score: [Add your value]

## File Structure

```
├── README.md                  # Project documentation
├── train_model.py             # Script for model training
├── app.py                     # Flask web application
├── templates/                 # HTML templates
│   └── index.html             # Prediction interface
├── static/                    # CSS, JS, and static assets
├── models/                    # Saved model files
│   └── ridge_house_price_model.pkl  # Trained model
├── requirements.txt           # Python dependencies
├── Procfile                   # Heroku deployment configuration
└── runtime.txt                # Python version for deployment
```

## Technical Details

### Preprocessing Steps

- Missing value imputation using mean and mode
- Standardization of lot sizes to consistent units
- Feature scaling for numerical stability
- One-hot encoding of ZIP codes

### Feature Engineering

- Price per square foot calculation
- Bedroom-bathroom ratio
- Standardized measurements

### Models Evaluated

- Ridge Regression
- ElasticNet
- Bagged Ridge Ensemble

## Deployment

The project includes configuration files for Heroku deployment:
- `requirements.txt`: Lists required packages
- `Procfile`: Specifies web server configuration
- `runtime.txt`: Defines Python version



