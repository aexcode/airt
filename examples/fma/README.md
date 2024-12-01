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

## Data Poisoning - SMS Spam Detection
* Load a free pre-trained sms spam detection model from Hugging Face
* Load an sms spam dataset and split into train and test
* Randomly poison a portion of the training data (change *poisoning_ratio* to alter level of poisoning) by flipping labels
* Fine-tune model by training on the now poisoned training data (this training session takes a little while; GPU will significantly improve training time)
* Evaluate the poisoned samples and classification failure rates based on portion poisoned data

