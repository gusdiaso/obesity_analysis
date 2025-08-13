# Trabalho 3 – Otimização do KNN com Evolução Diferencial e Enxame de Partículas

Este trabalho compara dois algoritmos de otimização – **Differential Evolution (DE)** e **Particle Swarm Optimization (PSO)** – para encontrar os melhores parâmetros do KNN.

## Objetivos

-   Comparar DE e PSO na otimização de hiperparâmetros do KNN.
-   Avaliar desempenho em dados originais e pré-processados.
-   Utilizar seleção de características com **SelectPercentile**.
-   Reduzir tempo de execução sem perda significativa de performance.

## Metodologia

1. Pré-processamento dos dados.
2. Seleção das 10 características mais relevantes com SelectPercentile.
3. Avaliação do KNN com **K-Fold Cross-Validation** (5 folds).
4. Otimização de parâmetros (n_neighbors, weights, p) usando DE e PSO.
5. Repetição por 30 execuções para avaliação robusta.

## Principais Resultados

-   Métricas (acurácia/F1/recall) muito próximas entre DE e PSO.
-   Dados originais: ~93% de acurácia; Pré-processados: ~92%.
-   Pré-processamento reduziu tempo de execução em mais de 50%.

## Estrutura

-   `codigo/` – Scripts e notebooks de otimização e análise.
-   `relatorio.pdf` – Relatório completo do trabalho.
