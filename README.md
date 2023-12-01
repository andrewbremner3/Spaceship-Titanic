# [Spaceship Titanic Classification](https://github.com/andrewbremner3/Spaceship_Titanic)
classification predictions from Kaggle competition [www.kaggle.com](https://www.kaggle.com/competitions/spaceship-titanic) where training and test data sets are provided.

**Goal: Predict if a passanger was transported based on the persons attributes and ticket information.**

### 1) Explore the Train data
Determine which fields are correlated to transport and which fields need to be preprocessed in order to be input into the machine learning models.

### 2) Train data Engineering
Fill empty data with the mode for catagorical fields and mean for numerical fields. Then convert the catagory values with 'dummy' values for input to the training model.

### 3) Repeat Data Engineering on Test data
Test data is held out until final steps.

### 4) Train various models with train data
Split training set into a train and test for the various models so I can check the accuracy of the models for comparison.

Models tested:
* RandomForestClassifier = 0.7987
* GradientBoostingClassifier = 0.7924
* HistGradientBoostingClassifier = 0.8039
* BaggingClassifier = 0.7797

### 5) Final Train and Output
The HistGradientBoostingClassifier has the best score from the tests so that is what is used in the final training set. Ouput the data as Kaggle needs the output for final testing.

The Final Score from the leaderboard = 0.79658.

