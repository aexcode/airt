# Attack Examples & Code

## Failure Mode Analysis

Examples here are created to demonstrate types of failure mode analysis. The [Microsoft guidelines on FMA](https://github.com/MicrosoftDocs/security/blob/main/security-docs/engineering/Failure-modes-in-machine-learning.md) are used to provide a set of terms and definitions. Code is provided as specific examples illustrating the FM type and a possible approach to exploitation.

### Perturbation
*Attacker modifies the query to get appropriate response*

[Example](fma/PerturbationExample_ImageClassifier.ipynb): A pretrained image classifier is given an image of an elephant. The image is then perturbed to add adversarial noise, which causes a misclassification.

