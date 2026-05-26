#  Avocado Price Prediction & Type Classification

## &#128279; Project Overview
This project applies supervised machine learning techniques to predict the price of avocados and the type of avocados using the Avocado dataset. 
There are multiple models that predict the price of avocadoes and multiple models that learn patterns that distinguish avocados into predefined labels (e.g., 'organic', 'conventional') 

## &#128279; Authors
* Ayomide Olatunde

## &#128279; Table of Contents
* [Authors](#-authors)
* [Table of Contents](#-table-of-contents)
* [Dataset Description](#-dataset-description)
* [Tools & Libraries Used](#-tools--libraries-used)
* [Workflow Implemented](#-workflow-implemented)
* [Exploratory Data Analysis](#-exploratory-data-analysis)
* [Model Performance](#-model-performance)
* [Key Insights](#-key-insights)
* [Learning Outcomes](#-learning-outcomes)
* [How to Run the project](#-how-to-run-the-project)
* [License](#-license)
* [Contact](#-contact)


## &#128194; Dataset Description
**Source**: avocado.csv
**Records**: 18249 entries
**Columns**: 14 

#### **Features Used**
- Date: Date of observation   
- AveragePrice: Average price of avocados   
- Total Volume: Total number of avocados sold   
- PLU codes (4046, 4225, 4770): Different avocado categories   
- Total Bags: Total number of bags sold   
- Type: Organic or Conventional   
- Region: Sales region   
- Year: Year of observation   

**Target Variable**    
Price Prediction:
- AveragePrice

Type of Avocado
- labels - 'conventional': 0, 'organic': 1   

## &#128736; Tools & Libraries Used

#### **Programming Language** : `Python 3.10+` 

#### Libraries
- `pandas` – Data manipulation & cleaning

- `numpy` - Numerical analysis

- `matplotlib & seaborn` – Data Visualization

- `scikit-learn (Logistic Regression, Linear Regression, PCA)` - Machine Learning

- `arima` - Time Series Analysis

#### Environment
- `Jupyter Notebook` - Interactive analysis & documentation

- `github`


## &#129529; Workflow Implemented

The following steps were performed for this project:  
1. Data Cleaning and Interrogation  
- Cleaning the column headers  
- Checking the information about the data (missingness, duplicates & data types)   
- Changing the data type of the date column and extracting the month   
- Dropping unnecesary column.  
- Checking for the statistical description of the data.  

2. Exploratory Data Analysis (EDA) 
- Distribution analysis of average price 
- Visualization of different feature patterns per target label across regions as well  

3. Data Preprocessing   
- Encoding of categorical variables   
- Correlation analysis between features and target 
- Train-Test-Split (80/20)
- Feature scaling (StandardScaler) 

3. Model Training (Supervised Learning)  
Trained the features on the following models:
- Linear Regression
- Time Series model
- Logistic Regression + PCA

4. Model Evaluation  
Models were evaluated using:   
- R2 score, RMSE and MAE for prediction  
- Accuracy, Precision, Recall, and F1-Score for classification  
- Confusion Matrix plot for classification  


## 📈 Exploratory Data Analysis  
- The distribution of the Average price was slightly right-skewed.  
- Organic avocados are more expensive and the least purchased.  
- Avocados were most expensive in 2017 and purchased the most in 2017.   
- Avocados were purchased more in February, May and July.   
- Avocados are most expensive in HartfortSpringfield region. Avocados are cheapest in Houston which borders Mexico.    
- The TotalUS and the West purchase the most avocadoes.   

## &#127942; Model Performance  
- For Price Prediction:     
| Model Name | R2 Score | RMSE |   
| --- | --- | --- |  
| Linear Regression | 0.315851 | 0.070294 |     
| Seasonal ARIMA | 0.386083	| 0.580103  |  

For Avocado Type Classification   
| Model Name | Accuracy Score | F1 Score | Recall Score | Precision Score |  
| --- | --- | --- | --- | --- |   
| Logistic Regression + PCA | 0.90 | 0.90 | 0.90 | 0.90 |  


## 🔍 Key Insights
- 1564 records were correctly predicted as Conventional Avocado type.    
- 123 records were incorrectly predicted as Conventional Avocado type
- 1707 records were correctly predicted as Organic Avocado type.  
- 256 records incorrectly predicted as Organic Avocado type.  


## &#127919; Real World Application  
- Forecasting the prices of Avocado and preparing towards it  
- For Farmers to know when to harvest & sell.   
- Better sorting of avocados   
- Agricultural research.  

## &#128161; Learning Outcomes
Through this project, I demonstrated proficiency in:

#### Technical Skills
- Data cleaning, analysis and preprocessing
- Exploratory data analysis techniques
- Correlation analysis and interpretation
- Data visualization (Matplotlib, Seaborn)
- Python programming for data science
- Jupyter Notebook documentation


#### Tools Mastered
- Python (Pandas, NumPy, Matplotlib, Seaborn, ScikitLearn)
- Jupyter Notebook
- Using different models  

## &#128640; How to Run the Project
1. **Python Installation** (3.10 or higher)
```windows cmd
py -m python --version
```

2. **Required Libraries**
```windows cmd
py -m pip install pandas numpy matplotlib seaborn scipy jupyter lab scikit-learn 
```

#### Step-by-Step Instructions

1. **Clone/Download Repository**
- Download the project folder
- Ensure all files are in the same directory

2. **Launch Jupyter Notebook**
```windows cmd
py -m jupyter lab
```

3. **Open the Notebook**
- Open `avocado.ipynb` In Jupyter.

4. **Run all cells at once or Run cells individually**

#### Troubleshooting

**Issue**: "File not found" error
**Solution**: Ensure `avocado.csv` is in the same directory as the notebook.

**Issue**: Import errors
**Solution**: Install missing libraries using `py -m pip install [library-name]`


## &#128222; Contact
- **Email**: ayomideeli2002@gmail.com
- **LinkedIn**: https://linkedin.com/in/ayomide-olatunde-2859141a8
- **GitHub**: https://github.com/mideolatunde

- **Institution**: She Code Africa Academy
- **Track**: Data Science
- **Facilitator**: Ifeoma Egbogah



