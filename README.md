# Linear Discriminant Analysis (LDA) Classification

This project demonstrates a manual implementation of Linear Discriminant Analysis (LDA) to classify synthetic 2D data from two Gaussian distributions.

## Objective
To implement Fisher’s Linear Discriminant for binary classification by projecting high-dimensional data onto a 1D axis that maximizes class separability.

## Dataset
- **Synthetic Data**: Two Gaussian-distributed classes with:
  - Shared covariance matrix
  - Means: Class 0 = [0, 0], Class 1 = [2, 2]
- Total samples: 200 (100 per class)

## Methodology
1. **Data Simulation**
   - Generated using `numpy.random.multivariate_normal`
2. **Fisher’s LDA**
   - Computed within-class and between-class scatter matrices
   - Derived optimal projection vector using `S_w^{-1}(μ_1 - μ_2)`
3. **Classification**
   - Projected data onto 1D axis
   - Applied threshold-based classification using midpoint of projected means
4. **Evaluation**
   - Accuracy score and confusion matrix
   - Visualization of class histograms and decision boundary

## Output
- Achieved near-perfect classification on linearly separable data
- Visualized the effectiveness of LDA projection in 1D

## Tools Used
- Python, NumPy, Matplotlib
- No external ML libraries (pure mathematical implementation)

## Author
Aahna Shresth  
[GitHub Profile](https://github.com/aahna-shresth)
