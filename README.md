# Spam Email Classifier- ( via Natural Language Processing and Supervised Learning Models)


## DEMO-

https://spam-emails-predict-via-nlp.herokuapp.com/

## Steps:

## Part 1: Data Collection-
  Dataset is taken from UCI website.
  

  Following are the links-
  

  https://archive.ics.uci.edu/ml/machine-learning-databases/00228/


  https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection
  
## Part 2: Data Modeling-
    
  Machine Learning Models used-
  
  
- Naive Bayes Model: 
  
  https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/Spam%20Classifier/Naive%20Bayes/Bayesian_Inference.ipynb
  
  
- Ensemble Machine Learning Model-

   Here, various ensemble models are used i.e.,- 
   
    BaggingClassifier
    
    RandomForestClassifier
    
    AdaBoostClassifier
   
   https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/Spam%20Classifier/Ensemble%20Machine%20Learning/Spam_%26_Ensembles.ipynb
   
## Part 3: Metrics Calculation-

https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/Spam%20Classifier/Classification%20with%20metrics/Classification_Metrics.ipynb

Here, different metrics for all the models(Naive Bayes, Random Forest, Boosting Calssifier, Adaboost Classifier, SVM) are calculated such as- 

  - Accuracy: 

  - Precision

  - Recall

  - F-1 Score

 And, it can be seen that Naive Bayes performed better than all the models in terms of Accuracy, Recall and F-1 score. Only for Recall metrics, Random Forest Classifier works best as shown below-

![alt text](https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/images/Metrics_Calculation_Image.PNG)

& their, Accuracy, Precision, Recall and F1 scores are compared at the end, with Naive Bayes model approach, which already performed very well on the data.

 Also, ROC Curve i.e., Receiver Operating Characteristic Curve)  to determine split, is calculated for all the models, and it can be seen that the ROC curve split can be best done in Naive Bayes model(96.82%), compared to other models. as shown below-

![alt text](https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/images/ROC_Score.PNG)

## Part 4: ROC Curves for the models-

#### i) Naive Bayes-

![alt text](https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/images/NB_roc.PNG)


#### ii) Random Forest Classifier-

![alt text](https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/images/RF_roc.PNG)

#### iii.) Adaboost Classifier-

![alt text](https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/images/Adaboost_roc.PNG)

#### iv.) Bagging Classifier-

![alt text](https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/images/Bag_roc.PNG)

## Part 5: NLP on models-

Applied Count Vectorizer and tfIdf Vectorizer on Random Forest and Gradient Boosting models-

https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/Spam%20Classifier/Natural%20Language%20Processing/MLClassifier_RandomForestModel_with_grid-search.ipynb

Precision: 1.0 , Recall: 0.83 , Accuracy: 0.977

https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/Spam%20Classifier/Natural%20Language%20Processing/MLClassifier_GradientBoostingModel_with_grid-search.ipynb

Precision: 0.913 , Recall: 0.857 , Accuracy: 0.97

## Part 6: Pickle file generated from trained model, placed under Flask Api-

https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/nlp_model.pkl


## Part 8: Test cases on deployed model-

- Spam Email:

Input-

![alt text](https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/images/spam-test-mail.PNG)

Output-

![alt text](https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/images/spam-test-mail-output.PNG)

- Ham Email:

Input-

![alt text](https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/images/ham-test-mail.PNG)

Output-

![alt text](https://github.com/rickhagwal/NLP-Spam-Email-Classifier/blob/master/images/ham-test-mail-output.PNG)

