### -------------------------------------------------------------------------------------------------------
# K-Nearest Neighbors - Classified Data
### -------------------------------------------------------------------------------------------------------
### K-Nearest Neighbors:
- an **algorithm**:
    - based on **Supervised Learning**
    - to solve **Regression and Classification problems**
    - where machines **learn with supervision**
    - **input data are labeled** and **expected output data is known**
    - with key **objective**:
    	- **to predict (classify) a categorical (qualitative) dependent output value (y)** based on **independent input variable(s) (x)** -> for **Classification problems**
    	- **to predict a continuous (quantitative) numeric dependent output value (y)** based on **independent input variable(s) (x)** -> for **Regression problems**
    - by **identifying the position of nearest neighboring observations**, we try:
    	- **to identify to which category, the new observation belongs to**
    	- **to find the best fit line (equation) that can be used to make predictions**
- **Regression and Classification analysis** are a **predictive modeling techniques**
- **Prediction algorithm for new observations**:
    - **Calculate the distance** from new observation (x) to all observations -> distance between new observations and old observations
    - **Sort the observations** by increasing distance from new observation (x)
    - **Predict the majority label of the K (KNN classifier)** closest observations
- **K (KNN classifier) value**:
    - **defines how many observations** we are going to look at, that **are next to the new observation (x)**
    - **affects the class of a new observation** -> to which class it will be assigned to
- **Scale of the variables** matters:
    - variables on a large scale - have a larger effect on the distance between the observations and on the K (KNN classifier)
    - variables on a small scale - have a smaller effect on the distance between the observations and on the K (KNN classifier)

### -------------------------------------------------------------------------------------------------------
### Project Objective: Predicting target class on classified data
Create a model that allows to put in a few features of classified data and returns back a prediction (classification) of a new observation by identifying the position of its nearest neighboring observations. Information about the classified data is in the dataset 'Classified_Data', with hidden feature column names (anonymized) and known target classes.

The Classified data dataset contains the following columns:
- **XVPM**
- **GWYH**
- **TRAT**
- **TLLZ**
- **IGGA**
- **HYKR**
- **EDFS**
- **GUUB**
- **MGJM**
- **JHZC**
- **TARGET CLASS**

### -------------------------------------------------------------------------------------------------------
### Table of Contents:
1. File Descriptions
2. Technologies Used
3. Structure of Notebook
4. Executive Summary

#### 1. File Descriptions
- K-Nearest Neighbors - Classified_Data.ipynb
- Classified_Data
- README.md

#### 2. Technologies Used
- Python
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Scikit-Learn

#### 3. Structure of Notebook
1. Import the Libraries
2. Load the Data
3. Exploratory Data Analysis
    - 3.1 Check out the Data
    - 3.2 Data Visualization
4. Data Preprocessing and Feature Engineering
    - 4.1 Identify the variables
    - 4.2 Dealing with Missing values
      - 4.2.1 Dealing with Missing values in Columns
      - 4.2.2 Dealing with Missing values in Rows
    - 4.3 Dealing with the Non-numerical features
    - 4.4 Standardize (Scale) the values of variables
5. Train and Test the K-Nearest Neighbors model
    - 5.1 Split the columns
    - 5.2 Split the data into Training dataset and Testing dataset
    - 5.3 Create the K-Nearest Neighbors model
    - 5.4 Train / fit the K-Nearest Neighbors model
    - 5.5 Predictions from the model on Testing data
    - 5.6 Evaluate the model on Testing data
      - 5.6.1 Classification report
      - 5.6.2 Confusion matrix
    - 5.7 Choose the best K (KNN classifier) value
    - 5.8 Re-create the K-Nearest Neighbors model
    - 5.9 Re-train / re-fit the K-Nearest Neighbors model
    - 5.10 Re-predictions from the model on Testing data
    - 5.11 Re-evaluate the model on Testing data
      - 5.11.1 Classification report
      - 5.11.2 Confusion matrix
    - 5.12 GridSearchCV
      - 5.12.1 Create the Grid of parameters
      - 5.12.2 Create the GridSearchCV model (Re-create the K-Nearest Neighbors (KNN) model)
      - 5.12.3 Train / fit the GridSearchCV model (Re-train / Re-fit the K-Nearest Neighbors (KNN) model)
      - 5.12.4 Predictions from the GridSearchCV model (Re-predictions from the K-Nearest Neighbors (KNN) model) on Testing data
      - 5.12.5 Evaluate the GridSearchCV model (Re-evaluate the K-Nearest Neighbors (KNN) model) on Testing data
      	- 1. Classification report
      	- 2. Confusion matrix

#### 4. Executive Summary
TBA
