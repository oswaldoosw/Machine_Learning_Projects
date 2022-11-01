# Forest_Cover_Type_Prediction
Since the dataset used in this project is very big (581k rows), PySpark is used over Pandas since it is very efficient for processing large datasets as it can perform distributed computation. Before training, a user-defined transform functionality is created to see if the models perform better with the addition of this functionality. Then, three classification algorithms are trained and fine-tuned to see which algorithm performs best. The result ends up with the Decision Tree Classifier performing the best among the three, with 84.6% accuracy on the test dataset.

#### Note: All explanations included in the .ipynb file.

## Package Installations
-       pip install pandas
       
-       pip install numpy  
  
-       pip install seaborn
 
-       pip install matplotlib
     
-       pip install findspark
 
-       pip install pyspark

## Acknowledgments
- <a href="https://archive.ics.uci.edu/ml/datasets/covertype">Forest Cover Type Dataset</a>
