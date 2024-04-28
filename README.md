
<h1 style="text-align:center;"> Marketing Budget Optimization using Machine learning</h1>
<p align="center">
  <img src="https://uploads-ssl.webflow.com/614248409efa35f4fda157dc/62464db2123a7a4921cb040c_campaign-budget-optimization.jpg" width="500" height="300">
</p>

# **Introduction**

A company specializing in B2C sales (product: Data Science and Data Engineering related courses) spends significant money on marketing campaigns across various channels such as social media, email, and search advertising. More information on marketing sources can be found in the data column “Marketing Source”. The marketing team faces challenges in optimizing the marketing budget allocation across these channels to maximize revenue and return on investment (ROI).<br><br>
This project aims to develop a data-driven approach to optimize the marketing budget allocation across various channels to maximize revenue and ROI. By using machine learning algorithms, the marketing team can make informed decisions about allocating the marketing budget based on predicted revenue and ROI.

## **Methods for Marketing Budget Optimization**


There are various ways to build a model for marketing budget optimization, and the choice depends on factors such as the data available, the complexity of the system, and the computational resources available. Some approaches are:


### **1. Rule-based systems:**
 In this approach, we typically look at budget proportion allocation based on predefined rules. Rule-based systems are easy to implement and interpret, but they may not be very accurate or adaptive. It makes sense to use them when you have a specific business mandate (example - ease of managing ads or segment of users you want to target).


### **2. Statistical techniques:**
 Statistical techniques such as correlation, probability are very helpful to find the righ budget mix for each marketing channel. In this approach, we use historical data to come up with priors and correlations to do budget allocation.


### **3. Linear optimizatiom:**
In this approach, we define the objective function(e.g. increase conversion, reduce total cost) and the constraints(e.g. we should not spend more than 1000$ on Instagram) to come up with a linear equation. The linear equation is usually solved using a solver such as Gurobi, Pulp, etc. for the right solution which gives the amount of money company needs to spend on each channel.


### **4. Machine learning:**
Machine learning systems combines strength of historical data and statistical techniques to explain the right channel for individual customers of the company. For example, a ML system can tell with a high confidence if a potentail customer will click on the ad or not.

### **Assumptions**

* We assume that <b>Interest Level</b> is our target variable which refers to the interest of a user for a lead id
* We assume that whenever the target variable is NA or Not called, the corresponding lead id is not meaningful and hence dropped
* If the model's prediction is very close to 1, it means that the user is very likely to engage with the lead id
* Columns with a lot of null values are not meaningful and imputation also won't be helpful


## Project Description

### Overview

In today's highly competitive market, our company specializes in B2C sales with a focus on delivering top-quality Data Science and Data Engineering courses. To effectively attract customers, a significant budget is allocated across various marketing channels including social media, email, and search advertising. The challenge lies in optimizing the marketing budget to maximize both revenue and return on investment (ROI).

This project aims to adopt a data-driven approach using machine learning algorithms to empower the marketing team with valuable insights for informed decision-making. The objective is to maximize revenue and ROI by optimally distributing the marketing budget across the most promising channels, thereby enhancing the overall business performance.

### Business Impact

- **Increased Product Conversions**: Targeting the right users through appropriate channels improves our product conversions, engaging more genuinely interested users.
- **Increased Revenue**: By effectively targeting users likely to engage and purchase, we enhance the probability of higher revenue.
- **Improved Budget Allocation**: Leveraging data and machine learning, we identify high ROI channels, optimizing budget allocation and reducing wastage.
- **Improved Customer Acquisition Cost (CAC)**: Targeting the most effective channels improves CAC and customer retention, enhancing profitability.

### Aim

The aim of this project is to leverage data-driven approaches and machine learning algorithms to optimize the allocation of the marketing budget across various channels, empowering the marketing team with the information needed for strategic decision-making.

## Data Description

The dataset includes:

- **Lead Id**: Unique identifier for each lead.
- **Lead Owner**: Internal salesperson associated with the lead.
- **Interest Level**: Level of interest of the lead, entered manually.
- **Lead Creation Date**: When the lead was generated.
- **Lead Location (Auto)**: Automatically detected lead location.
- **Creation Source**: Source of the lead generation.
- **Next Activity Date**: Scheduled date for the next activity with the lead.
- **Current Occupation**: Current profile or occupation of the lead.
- **Product Expectations**: Specific requirements or expectations of the lead.
- **Website Source**: Source through which the lead visited the website.
- **Lead Last Update Time**: Last update timestamp for the lead's information.
- **Marketing Source**: Marketing source that acquired the lead.
- **Lead Location (Manual)**: Manually entered location of the lead.
- **Demo Date**: Scheduled date for a product demo with the lead.
- **Demo Status**: Status of the booked demo.
- **Closure Date**: Date when the lead was successfully closed or converted.

## Tech Stack

- **Language**: Python
- **Libraries**: pandas, numpy, matplotlib, scikit-learn, xgboost, lightgbm

## Approach

### Exploratory Data Analysis (EDA)

- Understand the relationships between features and target variables.
- Identify and impute missing or invalid values.

### Data Preprocessing

- Encode variables using label encoding.
- Split the dataset into training and testing sets.

### Model Building and Testing

- Implement and test models such as Random Forest, Light Gradient Boosting, and Extreme Gradient Boosting.

## **Important Libraries**

* **pandas**: pandas is a fast, powerful, flexible, and easy-to-use open-source data analysis and manipulation tool built on top of the Python programming language. Refer to [documentation](https://pandas.pydata.org/) for more information.

* **NumPy**: The fundamental package for scientific computing with Python. Fast and versatile, the NumPy vectorization, indexing, and broadcasting concepts are the de-facto standards of array computing today. NumPy offers comprehensive mathematical functions, random number generators, linear algebra routines, Fourier transforms, and more. Refer to [documentation](https://numpy.org/) for more information. pandas and NumPy are together used for most of the data analysis and manipulation in Python.

* **Matplotlib**: Matplotlib is a comprehensive library for creating static, animated, and interactive visualizations in Python. Refer to [documentation](https://matplotlib.org/) for more information.

* **seaborn**: Seaborn is a Python data visualization library based on matplotlib. It provides a high-level interface for drawing attractive and informative statistical graphics. Refer to [documentation](https://seaborn.pydata.org/) for more information.

* **scikit-learn**: Simple and efficient tools for predictive data analysis
accessible to everybody and reusable in various contexts.
It is built on NumPy, SciPy, and matplotlib to support machine learning in Python. Refer to [documentation](https://scikit-learn.org/stable/) for more information.

* **Warnings**:The warnings library provides a way to handle warnings that are generated during program execution. Warnings are typically issued when there is a potential issue with code, but the code still runs without errors. The warnings module provides a way to catch these warnings and handle them in a way that is appropriate for the program. This can be especially useful when developing and debugging code, as warnings can help identify potential issues before they become errors.

* **sys**:The sys library provides access to some system-specific parameters and functions. This library can be used to access system-level information, such as the command line arguments passed to the program, the version of the Python interpreter being used, and more.

