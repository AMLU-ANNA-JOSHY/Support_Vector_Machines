# Support Vector Machine (SVM)

This repository contains notebooks related to Support Vector Machines (SVM). The general ideas, math and intuition behind, as well as implementations from scratch and using the scikit-learn library can be found.

## Intuition and Mathematics
- SVM is explained as a 'Maximum margin classifier'. I would like to picturize this as tying two rope boundaries to separate a group of cows from a group of sheeps. You try to maximize the gap between the two groups so that mixing is avoided, and finally draw a line right in the middle of the ropes. This line is the decision boundary of SVM, and the troublesome cows and sheeps touching the ropes and likely to mix up are the support vectors. So, the goal is to 'maximize the gap' or 'margin' for better classification. And the nearest samples or 'support vectors' influence the decision boundary.
- The technical explanations of the keyterms as well as theoritical explanations can be found in the ipynb notebook-1 shared. 
- The mathematics leading to the margin formulation, how it is implemented as an optimization problem, and the role of the regularization parameter 'C' that determines whether the margin is 'hard' or 'soft' can also be found in detail with figures and derivations in the notebook.

## Implementations
- SVM implementation using the scikit-learn library on common problems can be found in notebook-1 shared.
- Visualization of the decision boundary, comparison against logistic regression, and importance of parameter C are also included in this notebook.
- How non-linearity and multi-class problem are dealt in SVM are explained with project demos in notebook-2 shared.
- The importance of hyperparameter tuning and approaches used with implementation can also be found in this notebook.
- SVM can also be used for regression, whose implementation on the california housing dataset is included in notebook-3 shared.

## Key Learnings
### SVM use cases:
- Used for both classification and regression, especially with high-dimensional data such as images, and text.
- Implemented for smaller datasets with clear separations between the classes such as spam detection (Natural language processing), cancer detection (Bio-informatics), digit recognition (OCR) and face recognition (Computer Vision).
### Advantages and Limitations:
- SVM can handle non-linearities in data using kernel tricks.
- It can work in scarce data settings, compared to deep learning models.
- It requires less tuning than the deep models in low resource scenarios where there is a clear margin.
- But it can scale poorly to larger datasets compared to DL models.
- Also, where the data is noisy and has many outliers it works poor.
- Since it uses one-vs-one or one-vs-rest approaches to solve multi-class problems, this would add complexity.
