# Cat-vs-Dog
Binary Image Classifier
**Data Collection**: Gather a dataset consisting of labeled images of cats and dogs. Popular datasets for this task include the Kaggle Cats and Dogs dataset or your own curated collection.

**Data Preprocessing**:
- Resizing: Standardize the size of all images, typically to a smaller fixed size (e.g., 256x256 pixels) to ensure uniformity and reduce computational load.
- Normalization: Scale pixel values to a range of 0 to 1 by dividing by 255. This helps in faster convergence during training.

**Building the CNN Model**:
- Input Layer: Define the input shape based on the resized images.
- Convolutional Layers: Add several convolutional layers with filters to detect features. Each layer is followed by activation functions (ReLU) and pooling layers (MaxPooling) to reduce dimensionality.
- Flattening: Flatten the output from the convolutional layers to a one-dimensional vector.
- Fully Connected Layers: Add one or more dense layers to learn complex patterns. Used a dropout and batch normalization layer to prevent overfitting.
- Output Layer: Use a dense layer with a sigmoid activation function for binary classification (cat or dog).
