# Attack Examples & Code

**WORK IN PROGRESS**

## Failure Mode Analysis

Examples here are created to demonstrate types of failure mode analysis. The [Microsoft guidelines on FMA](https://github.com/MicrosoftDocs/security/blob/main/security-docs/engineering/Failure-modes-in-machine-learning.md) are used to provide a set of terms and definitions. Code is provided as specific examples illustrating the FM type and a possible approach to exploitation.

### Perturbation
*Attacker modifies the query to get appropriate response*

[Example](fma/PerturbationExample_ImageClassifier.ipynb): A pretrained image classifier is given an image of an elephant. The image is then perturbed to add adversarial noise, which causes a misclassification.


### Data Poisoning
*Injecting malicious data into training datasets to corrupt or bias the model.*

[Classification Example](fma/DataPoisoningExample-FeatureDetection.ipynb): The Iris dataset is used with two samples to illustrate poisoning datasets with a visualization of skewed results versus normal outputs

[SMS Spam Filter Example](fma/DataPoisoningExample-SMSSpamDetection.ipynb): A public SMS spam detection model is fine-tuned over a poisoned SMS spam dataset

[Weather Prediction Example](fma/DataPoisoningExample-WeatherPrediction.ipynb): A weather prediction example using the day of year as a predictor given temperature mins and maxes to provide an expected average

### Model Inversion
*Inferring or reverse engineering sensitive training data or parameters from model outputs.*

[Model Inversion Example](fma/ModelInversionExample-HandwritingDetection.ipynb): A basic example of the concept of model inversion against the MNIST handwriting digit dataset

[Adversarial Robustness Toolbox (ART) Model Inversion Example](https://github.com/Trusted-AI/adversarial-robustness-toolbox/blob/main/notebooks/model_inversion_attacks_mnist.ipynb): A more realistic and sophisticated walkthrough of model inversion from the Trusted AI ART notebooks. 
