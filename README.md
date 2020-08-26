# # parameter_optimization_dga_analysis



This repo contains works on classification of malicious and non-malicious URL using Machine Leraning by tuning the n_gram range.
To run the code snniptes:

```
pip install virtualenv
virtualenv mypython
pip install requirements_latest.txt
source mypython/bin/activate
```

  - The dataPreprocessing.zip file contains code for dataset modification
  - final__csv.csv contains the malicious and non-malicious URL labeled as 0 and 1
  - res.csv contains only benign URL(80 class)
  - Modified_final_updated_26_07_2020.ipynb contains all the necessary code for classification
  - accuracy_check.ipynb contains the functions for accuracy check called in Modified_final_updated_26_07_2020.ipynb 
  - cnn_1d.ipynb contains all the necessary code for classification using Convolutional neural network (1D)
  - tuning_logisticRegression.ipynb and tuning_svm.ipynb grid search to find the best parameters
  
# Tuning instructions

  - In order to check and run the n_gram range and ML Model run Modified_final_updated_26_07_2020.ipynb and change the variable below.
 Example 1:
n1 = 1 (n1 and n2 for N_gram rannge.e.g (1,1) will be unigram
n2 = 1
model_name = "LinearSVC"
 Example 2:
n1 = 2
n2 = 2
model_name = "MultinomialNB"
  - For CNN_1D run the cnn_1d.ipynb

