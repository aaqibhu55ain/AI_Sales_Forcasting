# AI-Driven Retail Demand Forecasting and Analytics Using Temporal Feature Engineering

An end-to-end machine learning pipeline for retail sales prediction using Walmart store sales data. This project demonstrates a complete workflow from data preprocessing to model deployment with real-time prediction capabilities.

## 📊 Project Overview

This research-backed system analyzes 11,000+ historical sales records and uses advanced feature engineering (40+ features) to build a Random Forest model achieving exceptional accuracy. The model is deployed through both a Streamlit web application and Power BI dashboard for business-level insights.

## 🎯 Key Features

- **Outstanding Accuracy**: Random Forest model achieving 0.9999 R² score and 97.79% accuracy (within 10%)
- **Low Error Metrics**: MAE of $38.99 and RMSE of $170.92
- **Comprehensive Feature Engineering**: 40+ engineered features including seasonality, holidays, and store-level indicators
- **Dual Deployment**: Streamlit app for real-time predictions + Power BI dashboard for analytics
- **Scalable Pipeline**: Handles 11,000+ historical records with robust preprocessing
- **Business-Ready**: Includes visualizations for seasonal trends, holiday spikes, and store-wise performance

## 📁 Project Structure

```
AI-sales-forecasting/
├── notebooks/
│   ├── 01_EDA_Walmart_Sales.ipynb          # Exploratory Data Analysis
│   ├── 02_Data_Preprocessing.ipynb         # Data cleaning and preprocessing
│   └── 03_Model_Building.ipynb             # Feature engineering & model training
├── data/
│   ├── raw/                    # Original Walmart sales dataset
│   └── processed/              # Cleaned and preprocessed data
├── requirements.txt            # Project dependencies
├── README.md                   # This file
└── research_paper.pdf         # Full research paper
```

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- pip or conda
- Jupyter Notebook

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/aaqibhu55ain/AI-sales-forecasting.git
   cd AI-sales-forecasting
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Download the dataset from Kaggle**
   - This project uses the **Walmart Store Sales Dataset** from Kaggle
   - Go to: https://www.kaggle.com/datasets/yasserh/walmart-dataset
   - Download all CSV files (train.csv, test.csv, stores.csv, features.csv)
   - Create folders: `data/raw/` and place the downloaded files there
   - The notebooks will automatically process the data into `data/processed/`
   
   **Note**: Due to file size limitations, the raw data files are not included in this repository. You must download them directly from Kaggle to run the notebooks.

### Running the Notebooks

Open and run the notebooks in sequence:

1. **01_EDA_Walmart_Sales.ipynb** - Explore the dataset and understand patterns
2. **02_Data_Preprocessing.ipynb** - Clean data and handle missing values
3. **03_Model_Building.ipynb** - Engineer 40+ features and train the Random Forest model

**Using Jupyter:**
```bash
jupyter notebook
```
Then navigate to the notebooks folder and open each notebook in order.

## 📈 Model Performance

| Metric | Value |
|--------|-------|
| **R² Score** | 0.9999 |
| **MAE (Mean Absolute Error)** | $38.99 |
| **RMSE (Root Mean Squared Error)** | $170.92 |
| **MAPE (Mean Absolute % Error)** | 5.20% |
| **Accuracy (within 10%)** | 97.79% |
| **Training Samples** | 11,000+ records |

### Top Feature Importance
1. Date-based features (month, week, year, season)
2. Store type and characteristics
3. Previous week sales (lag features)
4. Holiday and promotion indicators

## 🔧 Technology Stack

- **Data Processing**: Pandas, NumPy
- **Machine Learning**: Scikit-learn, Random Forest
- **Web App**: Streamlit
- **Visualization**: Power BI, Matplotlib, Seaborn
- **Notebooks**: Jupyter Notebook
- **Model Evaluation**: Scikit-learn metrics (RMSE, MAE, MAPE, R²)

## 📊 Data Overview

**Data Source**: [Kaggle - Walmart Store Sales Dataset](https://www.kaggle.com/datasets/yasserh/walmart-dataset)

- **Dataset**: Walmart Store Sales
- **Records**: 11,000+ weekly sales entries
- **Features Engineered**: 40+
- **Target Variable**: Weekly sales

### Raw Data Files (Download from Kaggle):
- `train.csv` - Historical training data
- `test.csv` - Test data for evaluation
- `stores.csv` - Store metadata (type, size, location)
- `features.csv` - Additional features (holidays, promotions, temperature)

### Feature Categories:
- Temporal features (month, week, year, season)
- Store-level features
- Lag and rolling average features
- Holiday and promotion indicators

## 📋 Methodology

1. **Exploratory Data Analysis** (01_EDA_Walmart_Sales.ipynb)
   - Dataset overview and statistical analysis
   - Visualization of sales patterns and trends
   - Correlation analysis

2. **Data Preprocessing** (02_Data_Preprocessing.ipynb)
   - Missing value handling
   - Outlier correction
   - Data scaling and normalization

3. **Feature Engineering & Model Training** (03_Model_Building.ipynb)
   - Creation of 40+ meaningful features
   - Model selection and comparison
   - Hyperparameter tuning
   - Performance evaluation

## 📊 Deployment

### Layer 1: Streamlit Web App
- Real-time input fields for sales prediction
- Interactive prediction output
- Embedded charts and insights
- User-friendly interface for quick predictions

### Layer 2: Power BI Dashboard
- Store-wise performance tracking
- Weekly trend analysis
- Forecast visualizations
- Profitability and demand heatmaps
- Executive-level analytics

## 🔮 Future Enhancements

- Integration of LSTM neural networks for time-series forecasting
- Real-time API data integration
- Cloud deployment (AWS/Azure)
- Advanced ensemble methods
- Mobile app interface
- Automated retraining pipeline

## 💡 Key Insights

- Seasonal trends significantly impact sales predictions
- Holiday periods show distinct sales spikes
- Store type and location are crucial predictors
- Previous week's sales (lag features) are strong indicators of future demand
- The model achieves 97.79% accuracy within a 10% prediction range

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues or pull requests to improve the project.

## 📧 Contact

**Author**: Aaqib Hussain Dar  
**Email**: dar.aaqib2019@gmail.com  
**GitHub**: [@aaqibhu55ain](https://github.com/aaqibhu55ain)
**LinkedIn**: https://www.linkedin.com/in/aaqibhu55ain/

For questions, collaboration, or feedback, feel free to reach out or open an issue on GitHub.

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

**Built with ❤️ for retail analytics and AI-driven decision making.**
