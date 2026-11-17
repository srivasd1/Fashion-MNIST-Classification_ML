# Fashion-MNIST Classification Using Machine Learning

## Project Overview

This project investigates the performance of three classical machine learning algorithms for classifying Fashion-MNIST images. The objective is to compare their classification accuracy, optimize model hyperparameters, and evaluate their performance against published state-of-the-art results.

## Dataset

The Fashion-MNIST dataset consists of 70,000 grayscale images (28 × 28 pixels) belonging to 10 clothing categories.

- Training dataset: 60,000 images
- Test dataset: 10,000 images
- Number of classes: 10
- Features: 784 pixel values per image

## Machine Learning Models

Three classification algorithms were implemented using Scikit-learn:

1. **Logistic Regression** – A linear classification model used as a baseline.
2. **Random Forest Classifier** – An ensemble learning algorithm combining multiple decision trees.
3. **Support Vector Classifier (SVC)** – A classification algorithm that identifies an optimal decision boundary between classes.

Hyperparameter optimization was performed using `GridSearchCV` with cross-validation.

## Model Evaluation

The models were evaluated using:

- Classification accuracy
- Precision, recall, and F1-score
- Confusion matrices
- Training and test accuracy comparisons

### Results

| Model | Test Accuracy |
|---|---|
| Logistic Regression | To be updated |
| Random Forest | 88.26% |
| Support Vector Classifier (SVC) | 90.11% |

The Support Vector Classifier achieved the highest test accuracy among the three evaluated models.

Both Random Forest and SVC achieved 100% training accuracy in the evaluated configurations, indicating a potential risk of overfitting. Further hyperparameter tuning and regularization could improve generalization.

## Comparison with Published Research

The classification results were compared with the work of Mukhamediev (2024), which reported 99.65% accuracy using a convolutional neural network (CNN-3-128) with data augmentation.

The comparison highlights the performance difference between classical machine learning algorithms and deep learning approaches for image classification.

## Technologies Used

- Python
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Future Improvements

- Explore additional SVC regularization parameters.
- Improve hyperparameter optimization.
- Investigate feature scaling and dimensionality reduction.
- Implement convolutional neural networks (CNNs) for comparison.
- Analyze misclassified images to identify model limitations.

## References

1. Xiao, H., Rasul, K., & Vollgraf, R. (2017). *Fashion-MNIST: A Novel Image Dataset for Benchmarking Machine Learning Algorithms.* [arXiv:1708.07747](https://arxiv.org/abs/1708.07747)

2. Mukhamediev, R. I. (2024). *State-of-the-Art Results with the Fashion-MNIST Dataset.* Mathematics, 12(20), 3174. https://doi.org/10.3390/math12203174
