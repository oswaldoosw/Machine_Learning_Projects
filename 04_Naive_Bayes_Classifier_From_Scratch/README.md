# Naive_Bayes_Classifier_From_Scratch
In this project, I created a Naive Bayes Classifier from scratch, which aims to predict abalone's age class. The <a href="https://archive.ics.uci.edu/ml/datasets/abalone">Abalone Dataset</a> comes with a continuous attribute called Rings. The dataset author suggests that Rings + 1.5 gives the abalone's age in years. Then, I created a new attribute called Age as the target, which contains the abalone's age, encoded into classes '1', '2', and '3'. Therefore, with three classes on the target attribute, this becomes a Multiclass Classification. 

A 70:30 ratio split is performed on the original dataset into train and test. Some procedures are performed, such as identifying the categorical and continuous attributes. Then, for every row in the training dataset, a calculation regarding the maximum likelihood for Age = 1, Age = 2, and Age = 3 is performed. The highest probability between all three classes is the prediction.

## How to Run the Classifier With Another Dataset?
### Step 1: Prepare Your Own Dataset
First off, delete these lines.
-       def categorize_age(df):
               if df['Age'] < 8:
                      return 1
               elif 8 <= df['Age'] <= 12:
                      return 2
               else:
                      return 3
-       df['Age'] = df['Rings'] + 1.5
        df['Age'].unique()
        df['Age'] = df.apply(categorize_age, axis = 1)

Then, proceed to change the path inside the read_csv's parameter and give column labels if needed.

-       df = pd.read_csv("./magic04.data", sep="," , header = None)
        df.columns = ['fLength','fWidth','fSize','fConc','fConc1', 'fAsym', 'fM3Long', 'fM3Trans', 'fAlpha', 'fDist', 'class']
        
Change the className variable to the target attribute of the dataset. In this magic04 dataset, the target is the column named class.
-       className = 'class'

For the dataframes df_train_x, df_train_y, df_test_x, and df_test_y, drop or pop the target attribute of the dataset.
-       df_train_x = df_trainn.drop(['class'], axis = 1)
        df_train_y = df_trainn.pop("class")
-       df_test_x = df_testt.drop(['Age'], axis = 1)
        df_test_y = df_testt.pop("Age")
        
Finally, run the whole notebook. This is the result of the magic04 dataset. <br/>
![image](https://user-images.githubusercontent.com/103481357/198844658-f4e5aca9-6410-453f-a9ed-f7e597a5b1c2.png) <br/>
![image](https://user-images.githubusercontent.com/103481357/198844667-6789ce00-1c47-4d3b-bf96-b8c256b3d874.png)

This result of this Naive Bayes Classifier lines up with the result of Scikit-Learn's Gaussian Naive Bayes Classifier. <br/>

![image](https://user-images.githubusercontent.com/103481357/198844696-5801f364-22b3-4865-87ba-30a42c6d6549.png)




## Package Installations
-       pip install numpy
       
-       pip install pandas  
  
-       pip install statistics

## Acknowledgements
<a href="https://towardsdatascience.com/continuous-data-and-zero-frequency-problem-in-naive-bayes-classifier-7784f4066b51">Continuous Data and Zero Frequency Problem in Naive Bayes Classifier</a>
