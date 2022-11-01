# Facial_Recognition_Using_VGGFace
This project is about facial recognition, a classification of 30 different people. A custom dataset is created and used for the model training, where 24 of the classes are famous individuals, and the remaining 6 classes are me and my acquaintances. Before the model training, the images are prepared by extracting the face using MTCNN and resizing them all to the same pixel size. The model is created by applying transfer learning, with <a href="http://www.robots.ox.ac.uk/~vgg/publications/2015/Parkhi15/parkhi15.pdf">VGGFace</a> as the base model. VGGFace is a pre-trained model, which has been tested on benchmark computer vision datasets, yielding very high accuracy (98.95% on the LFW dataset). Due to the small dataset, which only includes 20 images per person for training and 5 images per person for validation, the accuracy reaches 100% for both the training and validation datasets. However, this may not be the case when there is a significant increase in the number of classes and rows.


#### Note: All explanations included in the .ipynb file

#### Sample Input and Output: 
![image](https://user-images.githubusercontent.com/103481357/198273235-efce4fff-41f0-451f-adc5-0b9d9908a6fd.png)

## This Model Can Identify
#### Note: These are all famous individuals, except for the six individuals marked with (???)
- Alejandro Toledo, outputted as alejandro
- Alvaro Uribe, outputted as alvaro
- Andre Agassi, outputted as andre
- Ariel Sharon, outputted as ariel
- Arnold Schwarzenegger, outputted as arnold
- Bill Clinton, outputted as bill
- Colin Powell, outputted as colin
- David Beckham, outputted as david
- My acquaintance, outputted as dicky (???)
- Donald Rumsfeld, outputted as donald
- George W. Bush, outputted as george
- Gerhard Schroeder, outputted as gerhard
- Gloria Macapagal Arroyo, outputted as gloria
- Guillermo Coria, outputted as guillermo
- Hans Blix, outputted as hans
- Hugo Chavez, outputted as hugo
- Jack Straw, outputted as jack
- Jacques Chirac, outputted as jacques
- Jean Chretien, outputted as jean
- John Ashcroft, outputted as john
- John Negroponte, outputted as johnn
- My acquaintance, outputted as jonathan (???)
- Junichiro Koizumi, outputted as junichiro
- My acquaintance, outputted as kings (???)
- Kofi Annan, outputted as kofi
- Laura Bush, outputted as laura
- Luiz Inacio Lula da Silva, outputted as luiz
- My acquaintance, outputted as morgan (???)
- Myself, outputted as oswaldo (???)
- My acquaintance, outputted as wenling (???)

## Package Installations
-       pip install numpy
       
-       pip install pandas  

-       pip install matplotlib

-       pip install tensorflow

-       pip install Pillow
     
-       pip install mtcnn
 
-       pip install scikit-learn

-       pip install keras_vggface
  
-       pip install face-recognition

## Acknowledgments
- <a href="http://www.robots.ox.ac.uk/~vgg/publications/2015/Parkhi15/parkhi15.pdf">VGGFace</a> as the pre-trained base model
- Data was taken and selected from the <a href="http://vis-www.cs.umass.edu/lfw/">Labeled Faces in the Wild dataset</a>
