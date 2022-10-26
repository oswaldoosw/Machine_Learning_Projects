# Face_To_BMI_Prediction
In this project, I created a Support Vector Regression based model to predict the BMI of a person, given an image of them as the input. I obtained the data from the <a href="https://www.kaggle.com/datasets/davidjfisher/illinois-doc-labeled-faces-dataset">Illinois DOC labeled faces dataset</a>. The dataset comes with front and rear images of 68149 prisoners. The prisoners' data, such as their height and weight, are included in the CSV file. Face extraction from images is performed and then turned into a vector (face encodings). The data is split into train and test before training the SVR model. The SVR model achieved a Mean Absolute Error of 3.4 kg/m2 (Train Dataset) and 3.7 kg/m2 (Test Dataset).

#### Note: All explanations included in the .ipynb file

#### Sample Input and Output:<br/>
![image](https://user-images.githubusercontent.com/103481357/197967789-681c89e8-528b-43b1-b4a4-4cde50e7f868.png)


## Package Installations
-       pip install numpy
       
-       pip install pandas  
  
-       pip install face-recognition
 
-       pip install matplotlib
     
-       pip install ipython
 
-       pip install scikit-learn


## Acknowledgements
- <a href="https://www.kaggle.com/datasets/davidjfisher/illinois-doc-labeled-faces-dataset">Illinois DOC labeled faces dataset</a>
