🇧🇷 Português | 🇺🇸 [English](README.en.md)

# Estimativa de Níveis de Obesidade com Machine Learning

Três trabalhos de aprendizado de máquina sobre o mesmo conjunto de dados de hábitos alimentares e condição física, desenvolvidos na disciplina **Tópicos Especiais em Matemática e Computação (TEMC)** da Engenharia de Computação da UERJ.

## Dataset

- **Nome:** [Estimation of Obesity Levels Based On Eating Habits and Physical Condition](https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition) (UCI Machine Learning Repository)
- **Amostras:** 2.111 pessoas do México, Peru e Colômbia
- **Atributos:** 16 preditores + 1 classe alvo (`NObeyesdad`, nível de obesidade)

## Trabalhos

| # | Pasta | Técnicas | Resultado principal |
|---|---|---|---|
| 1 | [`pca-kbest-kmeans`](./pca-kbest-kmeans) | PCA, SelectKBest, K-Means, índice Davies-Bouldin | A redução de dimensionalidade melhorou o índice Davies-Bouldin em relação ao conjunto completo |
| 2 | [`knn-gridsearch-loo`](./knn-gridsearch-loo) | KNN, Grid Search, validação Leave-One-Out | Melhor configuração: `n_neighbors=1`; acurácia 1,0 com alerta de overfitting |
| 3 | [`knn-de-pso`](./knn-de-pso) | Evolução Diferencial (DE) e Enxame de Partículas (PSO), K-Fold, SelectPercentile | DE e PSO muito próximos; ~93% de acurácia nos dados originais; o pré-processamento reduziu o tempo de execução em mais de 50% |

Cada pasta traz o notebook (`codigo.ipynb`), o relatório em PDF e um README com objetivos, metodologia e resultados.

## Tecnologias

Python · pandas · scikit-learn · Jupyter

## Como executar

```bash
git clone https://github.com/gusdiaso/obesity_analysis.git
cd obesity_analysis
pip install pandas scikit-learn matplotlib jupyter
jupyter notebook pca-kbest-kmeans/codigo.ipynb
```

## Autor

Gustavo Dias de Oliveira · Engenharia de Computação, UERJ · [LinkedIn](https://www.linkedin.com/in/gusdiaso/)
