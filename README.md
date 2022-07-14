# Credit_Risk_Analysis

## Overview of Analysis 

The purpose of this analysis was to create 6 different machine learning models and determine which one is best for predicting credit card risk. 

## Results 

See below for the results of all 6 machine learning models which includes their balanced accuracy, precision, and recall scores. 

### Random Oversampling:

<img width="619" alt="OverSample_BAC" src="https://user-images.githubusercontent.com/101602688/178861376-923d9b4e-0919-43bb-92ff-39ed05b8d4b1.png">


<img width="737" alt="OverSample_IMB" src="https://user-images.githubusercontent.com/101602688/178861398-b5b6cfeb-48e0-4f7e-aaf3-1ebb905f8e0f.png">


* Balanced Accuracy: 0.6398437216722869
* Precision: Precision is very high for low risk loans and very low for high_risk loans.
* Recall: High Risk/Low Risk = .59/.69

### SMOTE Oversampling:

<img width="494" alt="SMOTE_BAC" src="https://user-images.githubusercontent.com/101602688/178861415-9f610f8d-a46f-4238-92e9-44d3fc5690a1.png">


<img width="733" alt="SMOTE_IMB" src="https://user-images.githubusercontent.com/101602688/178861433-de3916c6-16a1-4ca5-8fa3-7b49891925da.png">


* Balanced Accuracy: 0.6216172933512213
* Precision: The values here are identical to the random oversampling which indicates the model is very good at predicting who is actually at low risk of credit card defaults but poor at predicting who was actually at high risk. 
* Recall: High Risk/Low Risk = .59/.66

### Undersampling:

<img width="622" alt="UnderSample_BAC" src="https://user-images.githubusercontent.com/101602688/178861459-33843883-a3fd-4a46-8b19-ca5169fda71d.png">


<img width="886" alt="UnderSample_IMB" src="https://user-images.githubusercontent.com/101602688/178861486-d30ec0ff-f56e-49af-8cfa-e9566e4457bc.png">


* Balanced Accuracy: 0.6216172933512213
* Precision: Identical to the previous two models again. 
* Recall: High Risk/Low Risk = .60/.43

### Combination Over and Under Sampling:

<img width="574" alt="Combo_BAC" src="https://user-images.githubusercontent.com/101602688/178861507-99ad0d06-b39f-467a-b375-1726d77f6c28.png">


<img width="813" alt="Combo_IMB" src="https://user-images.githubusercontent.com/101602688/178861527-4a108c4b-f4e6-4209-862f-9c45dab5819d.png">


* Balanced Accuracy: 0.5159904274991842
* Precision: Identical to previous 3 models. 
* Recall: High Risk/Low Risk = .69/.58

### Balanced Random Forest Classifier

<img width="613" alt="BalancedRandomForest_BAC" src="https://user-images.githubusercontent.com/101602688/178861542-ecf07eab-0b27-47dd-9302-5f8846a78998.png">


<img width="764" alt="BalancedRandomForest_IMB" src="https://user-images.githubusercontent.com/101602688/178861561-3a48c4b2-fd62-4e92-bf44-fc0db0c25100.png">


* Balanced Accuracy: 0.7877672625306695
* Precision: High Risk/Low Risk = .04/1.00. This indicates the model is accurate when predicting low risk users but much better at predicting high risk users than the previous 3 models.
* Recall: High Risk/Low Risk = .67/.91

### Easy Ensemble Classifier

<img width="543" alt="EasyEnsemable_BAC" src="https://user-images.githubusercontent.com/101602688/178861592-84aa8e9b-ee16-4706-92a9-0bade6c48ca2.png">


<img width="858" alt="EasyEnsemable_IMB" src="https://user-images.githubusercontent.com/101602688/178861618-a12f712f-8ae3-4816-958d-aa2a3c2774d3.png">


* Balanced Accuracy: 0.925427358175101
* Precision: High Risk/Low Risk = .07/1.00
* Recall: High Risk/Low Risk = .91/.94. This model is clearly the most accurate as it has the highest precision for high risk and highest recall for high risk. 


## Summary

After reviewing all 6 models, the Easy Ensemble Classifier model is clearly the best at predicting high credit card risk. The model has a 92% accuracy score, significantly higher than all other models as none of them had an accuracy score above 78%. In addition, the precision and recall scores were higher than the 5 other models. In conclusion, I would recommend the Easy Ensemble Classifier model to predict credit card risk. 
