# Terminators


We first loaded the training data, which consists of grayscale images of carcasses and their corresponding scores. We then preprocessed the data by reshaping the images and normalizing the pixel values. The model architecture consists of two convolutional layers with max-pooling, followed by a flattening layer and two dense layers. The model is trained using the Adam optimizer and mean squared error loss. The validation performance is monitored, and the model is trained for 20 epochs. The final model is then used to predict the scores for the validation images, and the predicted scores are categorized into different grade categories based on predefined score ranges. Finally, we saved resulting data in csv file.

The reasoning behind this approach is to leverage the powerful feature extraction capabilities of CNNs to learn relevant patterns from the carcass images, and then use a regression-based approach to predict the scores. The categorical classification based on the predicted scores is a practical way to present the final results in a format that aligns with the industry standards.
