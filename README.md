# EmployeeAttrition
Training an AI model to perdict emplyee attrition.

-	Tried SMOTE and ADASYN for up-sampling by creating synthetic data, they were pretty much the same but SMOTE seemed a tiny bit better. NOTE: all files currently use SMOTE.  To use the ADASYN alg, just replace SMOTE with ADASYN (I think there are like 2 occurrences)
-	Upsampling test data gave better results, but it seems like it’s putting fake data in there. 
Method ^^: Tried downsampling the test data and upsampling the training data so that the testing data wouldn’t be synthetically increased at least.  Predicting “no” for attrition was ok, with the average being in the high 60s.  Predicting yes for attrition was worse, with the average being in the high 40s.
-	Adjusting the number of features selected from 20 to 25 improved overall results. 23 seems better.  22 lowest accuracy = 58, high 70. 14 Lowest accuracy was 61, high 70. K=13, L=57, upper=70

- "data_cleaning_and_model_trainingOLD.ipynb": the original working file with different options commented out - probably don't need to use this for the paper. It's mostly just for reference if we need it.
- "FINAL-data_cleaning_and_model_training.ipynb": this is the file we will want to submit for grading.
- "test-DS-train-US-data_cleaning_and_model_training.ipynb": testing data is down-sampled and training data is up-sampled
- "test-US-train-US-data_cleaning_and_model_training.ipynb": both testing and training data are up-sampled.
