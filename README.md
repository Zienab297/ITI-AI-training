# ITI-training
Two weeks of AI-intensive training
## Final project
Trained several models on the Diabetes dataset. <br/>
Explored the data checking for duplicates, nulls, and outliers. I used a box plot to detect outliers and found several in most columns. Applied quartile to normalize the data. To find relations between data visualized using pair plot and heat map.
### Dataset Description
The data contains 9 features <br/>
* Number of Pregnancies
* Glucose level
* Blood Pressure
* Skin Thickness
* Insulin Level
* BMI
* Diabetes Pedigree Function (Target for Regression)
* Age
* Outcome (Whether the person has diabetes or not)
### Principal Component Analysis(PCA)
PCA is a technique for dimensionality reduction that is used to improve model performance. It reduces the dimensions of the data preserving the original information. It works by transforming potentially correlated variables into a smaller set of variables, called principal components. This improved method improved accuracy and reduced the mean square error.
### Models
#### Linear Regression
Applied the ```train_test_split``` function to split data into the PCA components and the target column which is ``` Diabetes Pedigree Function``` and split them into train and test. The used model was ```LinearRegression``` built-in function from ```sklearn.linear_model```, then fitted the data on the train data. Ran the model on the X test set to predict the output. The mean square error resulted was ```0.0815```.
