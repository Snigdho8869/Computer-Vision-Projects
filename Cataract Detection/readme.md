# Cataract Detection

This project focuses on detecting cataracts in eye images using deep-learning models and visualization techniques. The process involves data splitting, model development, training, and visualization of activation maps and attention maps.

## Data Preprocessing

- Data is divided into training, validation, and test sets using a specified ratio.
- Image data augmentation is performed on the training set to improve model performance.

## Model Development

### InceptionV3 Transfer Learning

- A pre-trained InceptionV3 model with added custom layers is used for cataract detection.
- The model is compiled with categorical cross-entropy loss and the Adamax optimizer.

#### Model Training

- The model is trained on the training set, and its performance is evaluated on the validation set.
- Training and validation loss and accuracy are visualized using graphs.

#### Activation Map Visualization

- Activation maps are generated to visualize the feature maps produced by a specific layer of the model.
- Activation maps can help in understanding which areas of the image contribute to the model's decision.

#### Grad-CAM (Gradient-weighted Class Activation Map)

- Grad-CAM is used to generate an attention map for the input image.
- The attention map highlights the areas in the image that are crucial for the model's prediction.
- Attention maps provide interpretability and insight into the model's decision-making process.

### Custom CNN Model

- A custom CNN model is developed for cataract detection using similar procedures as the InceptionV3 model.

## Evaluation

- The models are evaluated on the training, validation, and test sets.
- Evaluation metrics include loss and accuracy.
- Sample images are loaded, and predictions are made to determine if the images show signs of cataracts.

## Results

- The Inception model achieves an accuracy of 97.36%
- The CNN model achieves an accuracy of 90.31%
