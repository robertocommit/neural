# Neural

[Kaggle Challenge Submission](https://www.kaggle.com/code/robimalco/home-credit-default-risk-pytorch-neural-network)

This Python script uses Pytorch to construct a Neural Network for predicting Home Credit Default Risk.

1. **Imports**: Required Python libraries for data processing, machine learning, and Pytorch are imported.
2. **Device Setup**: The script automatically detects whether a CUDA-capable GPU is available and sets the device accordingly.
3. **Hyperparameters**: The hyperparameters such as the test set size, number of epochs, batch size, learning rate and others are set.
4. **Data Loading**: The Home Credit Default Risk data is loaded from CSV files, specifically application_train.csv, application_test.csv and previous_application.csv.
5. **Data Preprocessing**: The data is preprocessed to be suitable for a neural network. This includes creating new custom features, handling missing values, standardising numerical features, and encoding categorical features.
6. **Data Splitting**: The processed data is split into training and validation datasets using a specified test size.
7. **Tensor Creation**: The training, validation, and test datasets are converted to Pytorch Tensors.
8. **Neural Network Model**: The neural network model is defined and instantiated. This includes an embedding layer for categorical variables, followed by multiple fully connected layers.
9. **Training**: The model is trained on the training data using the Adam optimizer and binary cross entropy loss for a specified number of epochs. The AUC and loss for each epoch are printed out.
10. **Validation**: The trained model is validated on the validation data. The AUC and loss are again printed out.
