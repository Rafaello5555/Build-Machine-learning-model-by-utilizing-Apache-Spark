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

Data Preparation step - : Trim those data down by removing an uninformative column and removing rows which do not have information about whether or not a flight was delayed. The next step of preparing the flight data has two parts: convert the units of distance, replacing the mile column with a kmcolumn; and
create a Boolean column indicating whether or not a flight was delayed. We Create a label column with a value of 1 indicating the delay was 15 minutes or more and 0 otherwise. Transform  2 categorical values "carrier" and "org"  into indexed numerical values. The final stage of data preparation is to consolidate all of the predictor columns into a single column.


Building the Model:  Next step is to build the model.  To objectively assess a Machine Learning model we need to be able to test it on an independent set of data. We can't use the same data that we used to train the model. The model will perform (relatively) well on those data. We will split the data into two components. Create a classifier object and fit it to the training data and make predictions for the testing data.   


Evaluate the model: We can assess the quality of the model by evaluating how well it performs on the testing data. Evaluate the performance of the model by using confusion matrix.  Count the number of True Negatives, True Positives, False Negatives and False Positives and  calculate the accuracy.
