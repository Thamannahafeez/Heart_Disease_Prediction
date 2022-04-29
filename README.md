# HeartDiseasePrediction
Problem description
Your goal is to predict the binary class heart_disease_present, which represents whether or not a patient has heart disease:
0 represents no heart disease present
1 represents heart disease present

The heart disease prediction file creates a supervised prediction model to predict whether the patient is having heart disease or not.
The dataset provided was in the form of two separate CSV files, one contained the features and the other the target.
The outliers are eliminated using the Interquartile range. 
The categorical features are encoded using the pandas get_dummies() function.
The correlation among the features is visualized using the heatmap, while the correlation between the features and the target variable is plotted using a bar graph.
The dataset is split into training and testing data using 'train_test_split' in a 70:30 ratio.
Column Transformer is used to scale the numerical variables for the efficient performance of our model.
Since we saw an imbalance in the target classes, we can apply smote to balance using the oversampling technique.
The features are selected using the SelectFrom Model where the features with high feature importance are selected and separated as a new training and testing dataset.
Three models are trained and tested against the data in our hand,
    -- Logistic Regression
    -- KNN
    -- Random Forest
After carefully evaluating and taking all the metrics into consideration the KNN algorithm was giving the best result.
Hyperparameter tuning was done but did not result in the improvement of the performance of the algorithm.
