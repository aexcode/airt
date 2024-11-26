## Perturbation - Image Classifier

* Load a pre-trained model MobileNetV2
* Load an image of an elephant that will normally be classified as indian_elephant
* Introduce noise (change the variable *epsilon* to alter the amount of noise introduced)
* Classify and note perturbation success at ~0.06 epsilon threshold; increase to observe ranges of misclassification (eg. triceratops, military uniform, jigsaw puzzle, etc.)

## Data Poisoning - Feature Detection
* Load the Iris dataset
* Select two features to attack as example (red & blue)
* Randomly poison a portion of the training data (change *poisoning_ratio* to alter level of poisoning) by flipping labels
*  Using Logistic Regression, demonstrate the shift in decision boundary based on poisoning ratio and visualize (eg at 20% poisoned inputs, boundary will shift to .88 avg accuracy from 1.00)
