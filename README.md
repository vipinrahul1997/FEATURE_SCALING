StandardScaler is a feature-scaling technique from scikit-learn that transforms numerical features so that they have:

Mean = 0
Standard deviation = 1

Why do we fit StandardScaler only on training data?
To prevent data leakage. If we calculate the mean and standard deviation using the test data, information from the test set indirectly enters the training process. 
Therefore, we calculate scaling parameters only from X_train and apply the same parameters to X_test.
