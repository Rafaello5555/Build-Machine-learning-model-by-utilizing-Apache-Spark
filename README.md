# Build-Machine-learning-model-by-utilizing-Apache-Spark
We can interact with  Spark by using different languages such as Python,R, Scala, Java.  I have used Python in this project. The project is about  developing  a model which will predict whether or not a given flight will be delayed. The data contain  50000 records. 

 Data dictionary:
mon — month (integer between 1 and 12)
dom — day of month (integer between 1 and 31)
dow — day of week (integer; 1 = Monday and 7 = Sunday)
org — origin airport 
mile — distance (miles)
carrier — carrier 
depart — departure time (decimal hour)
duration — expected duration (minutes)
delay — delay (minutes)


We  wrangle the data to see if we have missing values, categorical values. In a sense we make data preparation.  Next step is to build the model.  To objectively assess a Machine Learning model we need to be able to test it on an independent set of data. We can't use the same data that we used to train the model: of course the model will perform (relatively) well on those data. Train the data and fit it to the training dataset and make predictions based on the  model. At the end we evaluate the performance of the model using confusion matrix.  Calculate the elements of the confusion matrix and  get accuracy .
