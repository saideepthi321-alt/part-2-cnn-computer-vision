# part-2-cnn-computer-vision
## Task 1: Problem Identification

The given dataset represents an Image Classification problem.

In this dataset, each image belongs to one class only:
- normal
- scratch
- dent
- stain

The main goal is to give the correct label for the full image based on the defect present on the product surface.

This is not an object detection problem because there are no bounding boxes showing the defect location.

This is not a segmentation problem because there are no pixel-level masks for defects.

So, image classification is the correct problem type for this dataset.

A CNN model can learn different visual patterns like:
- scratch marks
- dent shapes
- stain areas
- normal surfaces

and classify the images into the correct category.

This type of problem is commonly used in manufacturing quality inspection systems to automatically detect defective products.

## Task 2: Dataset Exploration
The dataset contains four classes:
- normal
- scratch
- dent
- stain

Dataset exploration was performed to analyze:
- number of images per class
- sample images
- image dimensions
- class balance

Sample images and class distribution plots were generated in the notebook.

## Task 3: Image Preprocessing
The images were preprocessed before training the CNN model.

Preprocessing steps included:
- resizing images to 128x128
- normalization of pixel values
- train-test split
- data augmentation

These preprocessing steps help improve model performance and training stability.

## Task 4: CNN Model Creation
A CNN model was built using TensorFlow/Keras.

The model architecture includes:
- convolution layers
- ReLU activation
- max pooling layers
- flatten layer
- dense layers
- softmax output layer

The CNN model learns image features automatically for defect classification.

## Task 5: Model Training and Evaluation
The CNN model was trained on the manufacturing defect dataset.

Model evaluation included:
- training accuracy
- validation accuracy
- training loss
- validation loss
- confusion matrix
- sample predictions

The model successfully classified product surface defects into different categories.

## Task 6: CNN Concept Explanation
What is Convolution?

Convolution is a process where a small filter moves over the image to detect important features like:
- edges
- lines
- textures
- patterns

In CNN, convolution layers help the model learn visual features from images automatically.

For example:
- scratches
- dents
- stains

can be detected using convolution filters.

Why is Pooling Used?

Pooling is used to reduce the size of feature maps.

It helps:
- reduce computation
- reduce memory usage
- make the model faster
- avoid overfitting

The most common pooling method is Max Pooling, which keeps the most important feature values from small regions of the image.

Why is ReLU Commonly Used in CNNs?

ReLU stands for Rectified Linear Unit.

It is an activation function defined as:

f(x)=max(0,x)

ReLU converts negative values to 0 and keeps positive values unchanged.

It is commonly used because:
- it is simple and fast
- helps the model learn better
- reduces vanishing gradient problem
- improves training speed

Why are CNNs Better than Regular Feed-Forward Networks for Image Data?

CNNs are specially designed for image processing.

Compared to regular feed-forward neural networks, CNNs:
- automatically detect important image features
- require fewer parameters
- preserve spatial relationships in images
- perform better for image classification tasks

Regular feed-forward networks treat images as simple flat data, while CNNs can understand visual patterns and structures more effectively.

That is why CNNs are widely used in:
- image classification
- object detection
- medical imaging
- manufacturing defect detection
- facial recognition systems


## Task 7: Business Use Case Mapping
Manufacturing Quality Inspection

This computer vision solution can be used in the manufacturing industry for automatic quality inspection of products.

In factories, products may contain defects such as:
- scratches
- dents
- stains
- surface damage

Traditionally, workers manually inspect products, which can be:
- time consuming
- expensive
- less accurate for large-scale production

Using CNN-based image classification, cameras can capture product images and automatically detect defective products in real time.

Benefits of this solution:
- faster inspection process
- reduced human effort
- improved product quality
- reduced manufacturing defects
- increased production efficiency

For example, this type of system can be used in:
- automobile manufacturing
- electronics production
- mobile phone assembly
- metal surface inspection
- packaging industries

This shows how computer vision and CNN models can help industries improve automation and quality control processes.
