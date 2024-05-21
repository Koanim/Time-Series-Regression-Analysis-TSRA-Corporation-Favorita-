
<a name="readme-top"></a>

<div align="center">
  <h1><b>TIME SERIES REGRESSION ANALYSIS CORPORATION FAVORITA </b></h1>
</div>

<!-- TABLE OF CONTENTS -->

# 📗 Table of Contents

- [📗 Table of Contents](#-table-of-contents)
- Overview
- [🛠 Built With ](#-built-with-)
- [Tech Stack ](#tech-stack-)
- Packages and Libraries
- Cleaning The Data
- Exploratory Data Analysis
- Visualizations
- Analysis
- Findings
- [Key Insights ](#key-insights-)
- [💻 Getting Started ](#-getting-started-)
- [Prerequisites](#prerequisites)
- [Setup](#setup)
- [Install](#install)
- [Usage](#usage)
- [👥 Authors ](#-authors-)
- [🔭 Future Features ](#-future-features-)
- [🤝 Contributing ](#-contributing-)
- [⭐️ Show your support ](#️-show-your-support-)
- [🙏 Acknowledgments ](#-acknowledgments-)
- [📝 License ](#-license-)

<!-- PROJECT DESCRIPTION -->

# Predicting Sales for a Large Ecuadorian-based grocery retailer <a name="about-project"></a>

## Overview 

Machine learning and statistical methods like ARIMA and Prophet are vital tools for data scientists to predict and forecast sales. By analyzing data patterns, ML algorithms can uncover insights, identify trends, and draw meaningful conclusions.




## Data Sources 📊
- The dataset was provided in GitHub and SQL and was transformed to CSV format for transparency and reproductibility.
- Statistics on Time Series Regression Analysis Corporation Favorita.

## Topical Questions and Hypotheses

### Hypotheses 🔬:
#### A significance level (α) of 5% will used to perform all the hypothesis testing

-Null hypothesis : There is no significant difference in the sales of products on promotion and those not on promotion at Corporation Favorita.
- Alternative hypothesis: There is significant difference in the sales of products on promotion and those not on promotion at Corporation Favorita

 ### ANALYTICAL QUESTIONS 🤔: 
The following analytical questions will help us gain insight and as well as confirm our hypothesis

1. Is the train dataset complete (has all the required dates)?
2. Which dates have the lowest and highest sales for each year (excluding days the store was closed)?
3. Compare the sales for each month across the years and determine which month of which year had the highest sales.
4. Did the earthquake impact sales?
5. Are certain stores or groups of stores selling more products? (Cluster, city, state, type)
6. Are sales affected by promotions, oil prices and holidays?
7. What analysis can we get from the date and its extractable features?
8. Which product family and stores did the promotions affect.
9. What is the difference between RMSLE, RMSE, MSE (or why is the MAE greater than all of them?)
10. Does the payment of wages in the public sector on the 15th and last days of the month influence the store sales.




###Data Dictionary
Train_df
- ID - Uniquely identify each customer
- Sales - Amount of Sales made by the stores 
- Family - Different Store Categories 
- OnPromotion - Whether promotions was made
- Date - The date a sale was made 

Oil_df
- Daily oil price- which includes values during both the train and test data timeframes. 


Holidays_df
- Date : Date for the Holidays
- Type : Type of Holidays 
- Locale: The Geographical area for the holidays
- Locale Name : The name of the regions for the holidays
- Description : Information on the regions for the holidays
- Transferred : 


Stores_df

-Store_nbr : The Unique Identifier for the stores
-City : The City where the stores are located
-State : The state where the stores are located
-Type  :  The type of stores 
-Cluster : The grouping of similar stores


Transact_df
- date  : The date transactions were made
- store_nbr : The Unique Identifier for the stores 
- transactions : The amount of transactions made within the stores on that specific date 




## 🛠 Built With <a name="built-with"></a>

### Tech Stack <a name="tech-stack"></a>





<details>
<summary>Language</summary>
  <ul>
    <li><a href="https://www.python.org/">Python</a></li>
  </ul>
</details>


<details>
<summary>Database</summary>
  <ul>
    <li><a href="https://www.microsoft.com/en-us/sql-server">SQL</a></li>
  </ul>
</details>




## Packages and Libraries 📚
#### Collection of significant Python Libraries:
- Pandas
- Numpy
- Seaborn
- Scipy
- Matplotlib
- Pyodbc
- Dotenv
- Sklearn
- Scikit
- Imblearn
- Custom Imputer
- XG Boost
- Pipeline
-Statsmodel
-Pmdarima
-joblib

#Time Series Data Checklist

## Cleaning the Data 🧹
#### We begin by changing the  data types .
- Changing data types 
- Dealing with Nan values
- Replacing Values in categorical columns to be more consistent

## Exploratory Data Analysis 🕵



- Univariate Analysis
  https://github.com/Koanim/LP2-Telco-churn-prediction/blob/main/box%20plot.JPG


  
- Bivariate Analysis
- https://github.com/Koanim/LP2-Telco-churn-prediction/blob/main/bivariate.JPG?raw=true





## Visualizations 👀

- Line Chart 📈
- Bar chart 📊
- Calender Plot 
- Box Plot 
- Kernel Density Plot

## Analysis 🔍
- Utilizing Python and data analysis libraries such as Pandas, Matplotlib, and Seaborn, we performed exploratory data analysis (EDA) to uncover trends and insights.
- We analyzed sales by year,month on Family,Store_numbers and onpromotion.

##Statistical Models
- Sarima
-

## Machine Learning Models and Hyperparameter Tuning
-   Gradient_Boosting
-	XGBoost	
-   Linear_Regression	




## Findings 📈
- 0 sales were recorded on 1st of January  and 25th December for all years,clearly affirming there was no sales on those days as they were holidays 
- 2013 recorded low level of sales 
- Higher sales were recorded on saturdays and sundays

## Key Files 📂
- `TSRA-FAVORITA.ipynb`: Jupyter Notebook containing the code for data cleaning, EDA, and visualization.
- Raw data used for analysis.
>Train.csv
>Transactions.csv
>Store.csv
>Oil.csv
>Sample_Submissions.csv
>Holidays_events.csv
>Test.csv
-`README.md`: This file providing an overview of the project.



<p align="right">(<a href="#readme-top">back to top</a>)</p>
<!-- Features -->

## Key Insights <a name="key-features"></a>

- **Grocery1 represent the top sales by family**
- **Highest sales was recorded in December 2016**
- **Sales was HIgher after earthquake**


<p align="right">(<a href="#readme-top">back to top</a>)</p>










<!-- GETTING STARTED -->

## 💻 Getting Started <a name="getting-started"></a>


To get a local copy up and running, follow these steps.

### Prerequisites

In order to run this project you need:

- Python


### Setup

Clone this repository to your desired folder:


```sh
  cd my-folder
  git clone https://github.com/Koanim/Time-Series-Regression-Analysis-TSRA-Corporation-Favorita-.git
```

Change into the cloned repository

```sh
  cd  https://github.com/Koanim/Time-Series-Regression-Analysis-TSRA-Corporation-Favorita
  
```

Create a virtual environment

```sh

python -m venv env

```

Activate the virtual environment

```sh
    env/Scripts/activate
```


### Install

Here, you need to recursively install the packages in the `requirements.txt` file using the command below 

```sh
   pip install -r requirements.txt
```



<!-- AUTHORS -->

## 👥 Authors <a name="authors"></a>

- 🕵🏽‍♀️ **Victor Anim**                                [GitHub Profile](https://github.com/Koanim)   
- 🕵🏽‍♀️ **Aluko Oluwadamilola**                        [GitHub Profile](https://github.com/damzking?tab=repositories)
- 🕵🏽‍♀️ **Aminu Oluwarotimi Desmond**                  [GitHub Profile](https://github.com/bamzyyyy?tab=repositories)
- 🕵🏽‍♀️ **Nana Kwame Frimpong Baah**
- 🕵🏽‍♀️ **Leticia Blay**
- 🕵🏽‍♀️ **Richmond Tetteh**




<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTRIBUTING -->

## 🤝 Contributing <a name="contributing"></a>

Contributions, issues, and feature requests are welcome!

Feel free to check the [issues page](../../issues/).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- SUPPORT -->

## ⭐️ Show your support <a name="support"></a>

If you like this project kindly show some love, give it a 🌟 **STAR** 🌟

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGEMENTS -->

## 🙏 Acknowledgments <a name="acknowledgements"></a>

We acknowledge the following persons for their coaching and support

- Violette Naa Adoley Allotey
- Racheal Appiah-Kubi
- Israel Anaba Ayamga

<!-- LICENSE -->

## 📝 License <a name="license"></a>

This project is [MIT](./LICENSE) licensed.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

