# tmdb-box-office-prediction
**Problem: Predict overall worldwide box office revenue.**

**Input Data:** TMDB Box Office Prediction (https://www.kaggle.com/c/tmdb-box-office-prediction)

train.csv  
test.csv

**Target variable** - Revenue
**Independent variables** - include cast, crew, plot keywords, budget, posters, release dates, languages, production companies, and countries

**Language:** 
R, Python

**Steps followed:**

1. Understanding the data and story it tells  
2. Handling Missing Value  
3. Feature Engineering & Selection  
4. Splitting of data into training, validation, and testing  
5. Model fitting using h2o, xgboost, caret libraries from R  
6. Metrics comparison  

**Model used:**
Random Forest, XGBOOST, GBM, AUTO ML, also Keras DL model using python (in-complete)

**Output Files :**
1. R working files (code + rmarkdown output)  
2. Jupyter Notebook for Neural Network  
3. csv output files from different models (files are saved with model names)  

**Files Description:**

a) nanonets_assignment_html.Rmd - R Markdown file with R code  
b) nanonets_assignment_output.html - R Output  
c) nanonets_assignment.R - R script (Please Note - same as "a", only file type is different)  
d) test_output_rf.csv - test revenue predction using random forest  
e) test_output_xgboost.csv - test revenue predction using xgboost  
f) test_output_gbm.csv - test revenue predction using gbm  
g) test_output_aml.csv - test revenue predction using auto ml  
h) nn_bl_submission.csv - test revenue predction using baseline keras model (single layer)  
i) nn_1_submission.csv - test revenue predction using baseline keras model (input-hidden-output)  
j) clean_train.csv, clean_val.csv, clean_test.csv - final data after pre-processing in R, (input to the python jupyter notebook:- deep_learning_model.html)  
x) deep_learning_model.html - keras- dl model (in-complete)  


**Results:**

Model	    Log RMSE	  MAPE		  Corr b/w Actual & Prediction  
RF	      1.966068	  8.166273	0.7102687  
XGBOOST	  1.909717	  7.901881	0.725921  
GBM	      1.937532	  8.067186	0.7204951  
AutoML	  1.918164	  7.934945	0.723847  

