# Análise de Dados – Estimativa de Níveis de Obesidade

Este repositório contém três trabalhos desenvolvidos na disciplina **Tópicos Especiais em Matemática e Computação (TEMC)**, realizados por **Gustavo Dias de Oliveira**.  
Todos os trabalhos utilizam o dataset **"Estimation of Obesity Levels Based On Eating Habits and Physical Condition"** do repositório [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/544/estimation+of+obesity+levels+based+on+eating+habits+and+physical+condition).

O conjunto de dados contém informações sobre hábitos alimentares, condições físicas e estilos de vida de indivíduos do México, Peru e Colômbia, sendo utilizado para prever o **nível de obesidade**.

---

## Estrutura dos trabalhos

1. **[1-pca-kbest-kmeans](./1-pca-kbest-kmeans)**

    - Redução de dimensionalidade (PCA, SelectKBest)
    - Agrupamento não supervisionado (K-Means)
    - Avaliação da qualidade dos clusters (Davies-Bouldin Index)

2. **[2-knn-gridsearch-loo](./2-knn-gridsearch-loo)**

    - Classificação supervisionada (KNN)
    - Otimização de hiperparâmetros (Grid Search)
    - Validação cruzada Leave-One-Out (LOO)

3. **[3-knn-de-pso](./3-knn-de-pso)**
    - Comparação de métodos de otimização (Differential Evolution e Particle Swarm Optimization)
    - Avaliação com K-Fold Cross-Validation
    - Uso de SelectPercentile para seleção de atributos

---

## Dataset

-   **Nome:** Estimation of Obesity Levels Based On Eating Habits and Physical Condition
-   **Amostras:** 2.111
-   **Atributos:** 17 (16 preditores + 1 classe alvo)
-   **Classe alvo:** NObeyesdad (nível de obesidade)
-   **Origem:** UCI Machine Learning Repository

---

## Autor

-   **Nome:** Gustavo Dias de Oliveira
-   **Curso:** Engenharia da Computação – UERJ
