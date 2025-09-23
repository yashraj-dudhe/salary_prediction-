# Software Developer Salary Prediction System

## Overview
Built a comprehensive Streamlit-based machine learning application that predicts software developer salaries using Stack Overflow Developer Survey 2020 data. The system combines predictive modeling with interactive data visualization to provide insights into global salary trends.

## Project Description (Resume Format)
**Built a Streamlit-based ML system that predicts software developer salaries based on country, education, and experience using Stack Overflow survey data.**
• **Implemented a Decision Tree Regressor model** with hyperparameter optimization (max_depth=8) achieving accurate salary predictions across 14+ countries
• **Developed comprehensive data preprocessing pipeline** handling 30,000+ records with categorical encoding, outlier filtering, and feature engineering 
• **Created interactive web application** with dual functionality: real-time salary prediction and exploratory data analysis with dynamic visualizations
• **Deployed data visualization dashboard** featuring pie charts, bar charts, and line plots showing salary distributions by country and experience level

## Key Features

### 🔮 Salary Prediction
- **Interactive prediction interface** with dropdown menus and sliders
- **Real-time salary estimation** based on:
  - Country (14 supported countries including US, India, UK, Germany, Canada)
  - Education level (4 categories from "Less than a Bachelors" to "Post grad")
  - Years of experience (0-50 years)
- **Instant results** displaying predicted salary in USD

### 📊 Data Exploration & Analytics
- **Country-wise data distribution** with interactive pie charts
- **Salary analysis by country** using horizontal bar charts
- **Experience vs. Salary trends** with line chart visualization
- **Statistical insights** from Stack Overflow Developer Survey 2020

## Technical Implementation

### Machine Learning Pipeline
- **Model**: Decision Tree Regressor with optimized hyperparameters
- **Data Source**: Stack Overflow Developer Survey 2020 (30,000+ records)
- **Features**: Country, Education Level, Years of Professional Coding Experience
- **Target**: Annual Salary (USD)
- **Preprocessing**: 
  - Categorical encoding using LabelEncoder
  - Data filtering (salary range: $10k-$250k)
  - Experience normalization (handling edge cases like "More than 50 years")

### Technology Stack
- **Frontend**: Streamlit for interactive web interface
- **Machine Learning**: scikit-learn (Decision Tree Regressor)
- **Data Processing**: pandas, numpy
- **Visualization**: matplotlib, Streamlit native charts
- **Model Persistence**: pickle for model serialization

### Data Processing Features
- **Automatic category grouping** for countries with <400 responses
- **Education level standardization** across different degree types
- **Experience data cleaning** with special case handling
- **Real-time data filtering** and validation

## Screenshots

### Prediction Interface
![Salary Prediction Interface](https://github.com/yashraj-dudhe/salary_prediction-/assets/76808376/faf55500-9251-4d94-98c5-4da24b92cc6d)

### Data Exploration Dashboard
![Data Exploration Dashboard](https://github.com/yashraj-dudhe/salary_prediction-/assets/76808376/128e2d74-9316-4411-9d50-0a823eb6f46e)

## Installation & Usage

```bash
# Clone the repository
git clone https://github.com/yashraj-dudhe/salary_prediction-.git

# Install dependencies
pip install -r requirements.txt

# Run the application
streamlit run app.py
```

## Project Structure
```
salary_prediction/
├── app.py                 # Main Streamlit application
├── prdct.py              # Prediction page functionality
├── explore.py            # Data exploration page
├── project.ipynb         # Model development notebook
├── saved_steps.pkl       # Trained model and encoders
├── survey_results_public.csv  # Dataset
└── requirements.txt      # Dependencies
```

## Key Achievements
- ✅ **30,000+ data points** processed and analyzed
- ✅ **14 countries** supported for salary prediction
- ✅ **Real-time predictions** with sub-second response time
- ✅ **Interactive visualizations** for data exploration
- ✅ **Production-ready deployment** with Streamlit
- ✅ **Comprehensive data pipeline** with automated preprocessing

