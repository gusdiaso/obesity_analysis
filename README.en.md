🇧🇷 [Português](README.md) | 🇺🇸 English

# Obesity Level Estimation with Machine Learning

Three machine learning assignments on the same dataset of eating habits and physical condition, developed in the course **Special Topics in Mathematics and Computing (TEMC)** of the Computer Engineering program at UERJ.

## Dataset

- **Name:** [Estimation of Obesity Levels Based On Eating Habits and Physical Condition](https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition) (UCI Machine Learning Repository)
- **Samples:** 2,111 people from Mexico, Peru and Colombia
- **Attributes:** 16 predictors + 1 target class (`NObeyesdad`, obesity level)

## Assignments

| # | Folder | Techniques | Main result |
|---|---|---|---|
| 1 | [`pca-kbest-kmeans`](./pca-kbest-kmeans) | PCA, SelectKBest, K-Means, Davies-Bouldin index | Dimensionality reduction improved the Davies-Bouldin index compared to the full dataset |
| 2 | [`knn-gridsearch-loo`](./knn-gridsearch-loo) | KNN, Grid Search, Leave-One-Out validation | Best configuration: `n_neighbors=1`; accuracy 1.0, with an overfitting warning |
| 3 | [`knn-de-pso`](./knn-de-pso) | Differential Evolution (DE) and Particle Swarm Optimization (PSO), K-Fold, SelectPercentile | DE and PSO performed very similarly; ~93% accuracy on the original data; preprocessing cut execution time by more than 50% |

Each folder contains the notebook (`codigo.ipynb`), the PDF report (in Portuguese) and a README with objectives, methodology and results (in Portuguese).

## Tech stack

Python · pandas · scikit-learn · Jupyter

## How to run

```bash
git clone https://github.com/gusdiaso/obesity_analysis.git
cd obesity_analysis
pip install pandas scikit-learn matplotlib jupyter
jupyter notebook pca-kbest-kmeans/codigo.ipynb
```

## Author

Gustavo Dias de Oliveira · Computer Engineering, UERJ · [LinkedIn](https://www.linkedin.com/in/gusdiaso/)
