# part-2-cnn-computer-vision
## Task 1: Problem Identification

The given dataset represents an Image Classification problem.

In this dataset, each image belongs to one class only:
normal
scratch
dent
stain

The main goal is to give the correct label for the full image based on the defect present on the product surface.

This is not an object detection problem because there are no bounding boxes showing the defect location.

This is not a segmentation problem because there are no pixel-level masks for defects.

So, image classification is the correct problem type for this dataset.

A CNN model can learn different visual patterns like:

scratch marks
dent shapes
stain areas
normal surfaces

and classify the images into the correct category.

This type of problem is commonly used in manufacturing quality inspection systems to automatically detect defective products.

