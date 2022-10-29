# Naive_Bayes_Classifier_From_Scratch
In this project, I created a Naive Bayes Classifier from scratch, which aims to predict abalone's age class. The <a href="https://archive.ics.uci.edu/ml/datasets/abalone">Abalone Dataset</a> comes with a continuous attribute called Rings. The dataset author suggests that Rings + 1.5 gives the abalone's age in years. Then, I created a new attribute called Age as the target, which contains the abalone's age, encoded into classes '1', '2', and '3'. Therefore, with three classes on the target attribute, this becomes a Multiclass Classification. 

A 70:30 ratio split is performed on the original dataset into train and test. Some procedures are performed, such as identifying the categorical and continuous attributes. Then, for every row in the training dataset, a calculation regarding the maximum likelihood for Age = 1, Age = 2, and Age = 3 is performed. The highest probability between all three classes is the prediction.

## Package Installations

## Package Installations
-       pip install numpy
       
-       pip install pandas  
  
-       pip install statistics

## Acknowledgements
<a href="https://towardsdatascience.com/continuous-data-and-zero-frequency-problem-in-naive-bayes-classifier-7784f4066b51">Continuous Data and Zero Frequency Problem in Naive Bayes Classifier</a>
