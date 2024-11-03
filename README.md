# Stock-Price-Prediction-Using-Sentimental-Analysis
# Roadmap

### 1. **Define Project Goals**

- [x] Specific objectives: Predicting stock prices based on sentiment from news headlines.
      
### 2. **Data Collection**

- [x] **India News Headlines**: Collecting dataset from [Kaggle](https://www.kaggle.com/datasets/therohk/india-headlines-news-dataset)
- [x] **Stock Price Data**: Collecting dataset from [Kaggle](https://www.kaggle.com/code/taufiquesekh/stock-sentiment-analysis/input)
- [x] **Loading and Processing the Dataset**

### 3. **Data Preprocessing**

- [x] **Load Data**: Import news headlines and stock data from CSV files.
- [x] **Text Cleaning**: Clean headlines by converting to lowercase, removing non-alphanumeric characters, and eliminating stopwords.
- [x] **Sentiment Analysis**: Calculate sentiment scores (compound, positive, neutral, negative) using NLTK's VADER sentiment analyzer.
- [x] **Technical Indicators**: Compute stock indicators like SMA, EMA, MACD, RSI, and OBV to enhance feature set..

### 4. **Data Merging**

- [x] **Merge Datasets**: Combine processed sentiment data with stock data using the date field, forming a unified dataset for modeling.
      
### 4. **Sentiment Analysis with NLTK’s VADER sentiment analyzer.**

- [x] **Model Selection**: Choose a pre- [ ]trained VADER model
- [x] **Encoding Tweets** : Function to Preprocess headlines: Implement a function to encode headlines for input into the VADER model. This function performs several key operations:

### 3. **Rolling Window Forecasting**

- [x] **Set Window Size**: Define a rolling window size (e.g., 30 days) to train the model on past data for each prediction.
- [x] **Feature Scaling**: Standardize feature values for model input using `StandardScaler`.
- [x] **Model Training**: Utilize a `RandomForestRegressor` model to predict stock prices within each window.

### 4. **Model Evaluation**

- [x] **Calculate Metrics**: Assess model performance using MAE, RMSE, and R² scores to evaluate prediction accuracy.
- [x] **Print Results**: Output performance metrics for a final view of the model’s accuracy.

### 7. **Ensemble Model Creation**

- [ ] Combine predictions from LSTM, and Random Forest (e.g., via stacking or averaging).
- [ ] Test the ensemble model's performance against individual models.

### 8. **Deployment Preparation**

- [ ] **Environment Setup**: Prepare a deployment environment (e.g., Docker, virtual environments).
- [ ] **Model Serialization**: Save the trained models using libraries like `joblib` or `pickle`.

### 9. **Web Application Development**

- [ ] **Choose a Framework**: Decide on a web framework (e.g., Flask or Django).
- [ ] **Build APIs**: Create RESTful APIs to serve model predictions.
  - [ ] Endpoint to accept stock tickers and related text.
  - [ ] Endpoint to return predicted prices and sentiment scores.
- [ ] **Frontend Development**: Develop a user- [ ]friendly frontend (e.g., using HTML/CSS/JavaScript frameworks like React or Vue.js).
- [ ] **Integrate Models**: Connect your web app to the ensemble model to fetch predictions.

### 10. **Testing**

- [ ] Conduct thorough testing of the web application (unit tests, integration tests).
- [ ] Ensure the models return accurate predictions and handle various inputs.
