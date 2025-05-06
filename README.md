# Predictive-Analysis
*COMPANY*: CODTECH IT SOLUTIONS

*NAME*:CHAITANYA NAMDEO

*INTERN ID*:CT04DL130

*DOMAIN*:DATA ANALYTICS

*DURATION*:4 WEEKS

*MENTOR*:NEELA SANTHOSH 

*Description of the Pima Indians Diabetes Classification Script*
This Python script performs a machine learning classification task on the Pima Indians Diabetes dataset, aiming to predict whether a patient has diabetes based on medical attributes. The workflow includes the following steps:
1.Import Libraries: Loads essential Python libraries for data analysis, visualization, preprocessing, and modeling.
2.Load Dataset: Reads the dataset from a CSV file, assigning meaningful column names corresponding to medical measurements and the diabetes outcome.
3.Exploratory Data Analysis (EDA):Displays the first few rows and summary statistics of the dataset.
Visualizes the distribution of the target variable (Outcome) using a count plot.
4.Feature Selection:Separates features (X) from the target variable (y).
Standardizes features using StandardScaler to normalize the scale.
Applies SelectKBest with ANOVA F-statistics (f_classif) to choose the top 5 most relevant features for predicting diabetes.
5.Train/Test Split: Divides the dataset into training and testing sets (80/20 split) to evaluate the model's performance.
6.Model Training: Trains a Random Forest Classifier, a powerful ensemble learning method, using the selected features.
7.Model Evaluation:Predicts outcomes on the test set.
Prints the confusion matrix, classification report (precision, recall, F1-score), and overall accuracy to assess model performance.
This script is a practical example of a complete machine learning pipeline—from data loading and preprocessing to feature selection, training, and evaluation—for binary classification problems in healthcare analytics.

*OUTPUT*:
   Pregnancies  Glucose  BloodPressure  SkinThickness  Insulin   BMI  \
0            6      148             72             35        0  33.6   
1            1       85             66             29        0  26.6   
2            8      183             64              0        0  23.3   
3            1       89             66             23       94  28.1   
4            0      137             40             35      168  43.1   

   DiabetesPedigreeFunction  Age  Outcome  
0                     0.627   50        1  
1                     0.351   31        0  
2                     0.672   32        1  
3                     0.167   21        0  
4                     2.288   33        1  
       Pregnancies     Glucose  BloodPressure  SkinThickness     Insulin  \
count   768.000000  768.000000     768.000000     768.000000  768.000000   
mean      3.845052  120.894531      69.105469      20.536458   79.799479   
std       3.369578   31.972618      19.355807      15.952218  115.244002   
min       0.000000    0.000000       0.000000       0.000000    0.000000   
25%       1.000000   99.000000      62.000000       0.000000    0.000000   
50%       3.000000  117.000000      72.000000      23.000000   30.500000   
75%       6.000000  140.250000      80.000000      32.000000  127.250000   
max      17.000000  199.000000     122.000000      99.000000  846.000000   

              BMI  DiabetesPedigreeFunction         Age     Outcome  
count  768.000000                768.000000  768.000000  768.000000  
...
25%     27.300000                  0.243750   24.000000    0.000000  
50%     32.000000                  0.372500   29.000000    0.000000  
75%     36.600000                  0.626250   41.000000    1.000000  
max     67.100000                  2.420000   81.000000    1.000000  
![image](https://github.com/user-attachments/assets/0fb71464-39e1-401e-9050-1fc44b51ade2)

Selected features: ['Pregnancies', 'Glucose', 'BMI', 'DiabetesPedigreeFunction', 'Age']
Confusion Matrix:
 [[81 18]
 [17 38]]
Classification Report:
               precision    recall  f1-score   support

           0       0.83      0.82      0.82        99
           1       0.68      0.69      0.68        55

    accuracy                           0.77       154
   macro avg       0.75      0.75      0.75       154
weighted avg       0.77      0.77      0.77       154

Accuracy Score: 0.7727272727272727



