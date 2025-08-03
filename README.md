# Predictive Analysis of Restaurant Inventory: A Study on Stocking Items Based on Popularity Trends

## 📋 Project Overview

This project implements a comprehensive predictive analytics solution for restaurant inventory management using multiple machine learning models. The system forecasts restaurant demand patterns to optimize inventory stocking decisions, minimize food waste, prevent stockouts, and maximize profitability.

### 🎯 Key Objectives

- **Demand Forecasting**: Predict future sales quantities for different food items
- **Inventory Optimization**: Determine optimal stocking levels based on popularity trends
- **Waste Reduction**: Minimize food wastage through accurate demand prediction
- **Operational Efficiency**: Enhance restaurant operational efficiency and customer satisfaction

## 🚀 Features

- **Multi-Model Approach**: Implements 4 different forecasting models for comprehensive analysis
- **Time Series Analysis**: Advanced time series decomposition and pattern recognition
- **Seasonal Patterns**: Captures daily, weekly, monthly, and yearly seasonal variations
- **Performance Evaluation**: Comprehensive model comparison using multiple metrics
- **Visual Analytics**: Interactive plots and forecasting visualizations

## 🛠️ Tech Stack

### Programming Languages
- **Python 3.8+**

### Machine Learning & Data Science Libraries
- **TensorFlow/Keras** - Deep learning framework for LSTM implementation
- **Prophet** - Facebook's time series forecasting library
- **Statsmodels** - Statistical modeling for ARIMA and ETS
- **Scikit-learn** - Machine learning utilities and preprocessing
- **Pandas** - Data manipulation and analysis
- **NumPy** - Numerical computing
- **Matplotlib/Seaborn** - Data visualization
- **Plotly** - Interactive visualizations

### Development Tools
- **Jupyter Notebook** - Interactive development environment
- **GitHub** - Repository hosting

## 📊 Models Implemented

### 1. Long Short-Term Memory (LSTM)
- **Accuracy**: 92.14% (Quantity-wise prediction)
- **Specialized RNN architecture** for sequential data
- **Hyperparameter tuning** with Keras Tuner
- **Min-Max scaling** for data normalization

### 2. Prophet Model
- **Accuracy**: 68.14% (Individual pizza-wise prediction)
- **Facebook's open-source forecasting tool**
- **Decomposable additive model** (trend + seasonality + holidays)
- **Handles multiple seasonal periods**

### 3. Holt-Winters Exponential Smoothing (ETS)
- **Accuracy**: 79.99% (Quantity-wise prediction)
- **Triple exponential smoothing**
- **Captures level, trend, and seasonality**
- **Grid search hyperparameter optimization**

### 4. AutoRegressive Integrated Moving Average (ARIMA)
- **Accuracy**: 82.16% (Quantity-wise prediction)
- **Statistical time series model**
- **Seasonal decomposition and stationarity testing**
- **Automated parameter selection**

## 📁 Project Structure

```
Predictive-Analysis-of-Restaurant-Inventory_Big-data-Project/
├── Code/
│   ├── Arima_model/
│   ├── ETS_model/
│   ├── LSTM_model/
│   └── Prophet_model/
├── Results/
│   ├── Arima_model_results/
│   ├── ETS_model_results/
│   ├── LSTM_model_results/
│   └── Prophet_model_results/
└── README.md
```

## 🔧 Installation & Setup

### Prerequisites
```bash
Python 3.8 or higher
pip package manager
```

### Clone Repository
```bash
git clone https://github.com/chaitra-v26/Predictive-Analysis-of-Restaurant-Inventory_Big-data-Project.git
cd Predictive-Analysis-of-Restaurant-Inventory_Big-data-Project
```

### Install Dependencies
```bash
pip install tensorflow
pip install prophet
pip install statsmodels
pip install scikit-learn
pip install pandas
pip install numpy
pip install matplotlib
pip install seaborn
pip install plotly
pip install jupyter
pip install keras-tuner
```

### Alternative Installation (Requirements File)
Create a `requirements.txt` file with the above packages and run:
```bash
pip install -r requirements.txt
```

## 🚀 How to Run

### 1. Data Preparation
- The project uses synthetically generated data based on the Kaggle Pizza Sales dataset
- Ensure your dataset contains columns: `order_date`, `quantity`, `pizza_name`, etc.

### 2. Running Individual Models

#### LSTM Model
```bash
cd Code/LSTM_model/
jupyter notebook lstm_inventory_prediction.ipynb
```

#### Prophet Model
```bash
cd Code/Prophet_model/
jupyter notebook prophet_inventory_prediction.ipynb
```

#### ETS Model
```bash
cd Code/ETS_model/
jupyter notebook ets_inventory_prediction.ipynb
```

#### ARIMA Model
```bash
cd Code/Arima_model/
jupyter notebook arima_inventory_prediction.ipynb
```

### 3. View Results
Navigate to the respective results folders to view:
- **Forecast visualizations**
- **Performance metrics**
- **Model comparison charts**
- **Accuracy reports**

## 📈 Performance Metrics

### Quantity-wise Prediction
| Model | MSE | RMSE | MAPE | Accuracy |
|-------|-----|------|------|----------|
| **LSTM** | 10,754.83 | 103.70 | 7.86% | **92.14%** |
| Prophet | 111.98 | 10.51 | 32.84% | 67.15% |
| ARIMA | 41,460.16 | 203.62 | 17.84% | 82.16% |
| ETS | 58,396.04 | 241.65 | 20.01% | 79.99% |

### Individual Pizza-wise Prediction
| Model | MSE | RMSE | MAPE | Accuracy |
|-------|-----|------|------|----------|
| **Prophet** | 106.19 | 10.24 | 31.85% | **68.14%** |
| ETS | 106.81 | 10.28 | 32.04% | 67.96% |
| LSTM | 115.62 | 10.69 | 33.58% | 66.42% |
| ARIMA | 129.02 | 11.36 | 35.51% | 66.35% |

## 🔮 Future Enhancements

- [ ] **Real-time Data Integration**: Connect with POS systems for live data
- [ ] **Geographical Factors**: Include location-based demand patterns
- [ ] **Weather Integration**: Incorporate weather data for better predictions  
- [ ] **Ingredient Availability**: Factor in supply chain constraints
- [ ] **Customer Preferences**: Include demographic and preference data
- [ ] **Anomaly Detection**: Implement sudden demand spike detection
- [ ] **Mobile Application**: Develop restaurant management mobile app
- [ ] **Cloud Deployment**: Deploy models on cloud platforms

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 👥 Authors

- **Abhishek Bhat** - *CSE(AIML)* - abhishekbhat020@gmail.com
- **Vidhathri V** - *CSE(AIML)* - vvidha32023@gmail.com  
- **C Hemachandra** - *CSE(AIML)* - chinthimihemachandra1@gmail.com
- **Chaitra V** - *CSE(AIML)* - chaitrav2020@gmail.com
- **Lakshmi Snigdha Paladugula** - *CSE* - snigdha1012@gmail.com

## 🏛️ Institution

**PES University, Bangalore, India**  
Department of Computer Science and Engineering (Artificial Intelligence and Machine Learning)

## 📚 References

1. [Top 10 Challenges in Restaurant Inventory Management](https://www.fieldos.co/blog/top-10-challenges-in-restaurant-inventory-management)
2. [Pizza Sales Dataset - Kaggle](https://www.kaggle.com/datasets/shilongzhuang/pizza-sales)
3. Facebook Prophet Documentation
4. TensorFlow LSTM Documentation
5. Statsmodels Time Series Analysis

---
