# CS334-ML-Project

### Overview & Motivation:
Heart disease is the leading cause of death for people of most racial and ethnic groups all around the world over the past few decades. According to the data from Centers for Disease Control and Prevention, More than 600,000 Americans die of heart disease each year - that is one in every four deaths in this country. Moreover, about one in five people who had experienced a heart attack were not aware of it when the damage was done. If more people among them can be conscious of and predict the potential risk of heart disease, they are more likely to get an early diagnosis and prompt management of the disease.\
\
This project aims to create a prediction model to forecast the probability of developing heart disease so as to help individuals be aware of their own health risk and to help doctors make accurate and reliable diagnosis more quickly.
The dataset is from UCI Machine Learning Repository, which is the largest heart disease dataset available so far for research purposes. We are going to process and analyze the complex medical data related to heart disease with the help of machine learning techniques including some supervised learning algorithms such as K-Nearest Neighbor, Decision Tree, Support Vector Machine, Random Forest, and Naïve Bayes. 

![image](https://user-images.githubusercontent.com/60250593/138505232-1aa76192-9998-45e6-8ac6-39e1bb415cf1.png)


### Description:
The dataset we decided to use is the Heart Failure Prediction Dataset from University of California Irvine. This dataset was created by combining five independent dataset, which made it the largest heart disease dataset so far for research purposes. The dataset contains one csv file with 12 columns and 918 records. The complete description of each feature and its corresponding possible value is listed below:

- Age: age of the patient [years]
- Sex: sex of the patient [M: Male, F: Female]
- ChestPainType: chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]
- RestingBP: resting blood pressure [mm Hg]
- Cholesterol: serum cholesterol [mm/dl]
- FastingBS: fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]
- RestingECG: resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]
- MaxHR: maximum heart rate achieved [Numeric value between 60 and 202]
- ExerciseAngina: exercise-induced angina [Y: Yes, N: No]
- Oldpeak: oldpeak = ST [Numeric value measured in depression]
- ST_Slope: the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]
- HeartDisease: output class [1: heart disease, 0: Normal]

Since this is a classification problem (presence or absence of cardiovascular disease), we will be training and tuning K-Nearest Neighbor, Decision Tree, Support Vector Machine, Random Forest, and Naive Bayes models on the dataset, and try to find the best model for our problem.

#### Procedure:
We will be splitting 70000 records into two portions: the training set and the testing set. We will use all of the data to train and test, but not at the same time. We will 1. First use cross validation techniques such as k-fold cross validation or monte-carlo cross validation to train the model using the training set and tune the hyperparameters; 2. Use the best hyperparameter value to train the model using the entire training dataset; 3. Evaluate the model (model assessment) using the test dataset and different evaluation metrics such as accuracy score and F-1 score; 4. Train the model using the best hyperparameter we found and the entire train and test dataset. 


#### References:
There are totally 63 code submissions using our dataset on Kaggle. Most of them focused on data visualization and prediction model training. So far, the best model we could find on Kaggle is using the Random Forest model with a 90.2% accuracy score by SVEN ESCHLBECK.
