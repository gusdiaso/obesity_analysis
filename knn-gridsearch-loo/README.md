# Trabalho 2 – Classificação KNN com Grid Search e Leave-One-Out

Este trabalho aplica o algoritmo **K-Nearest Neighbors (KNN)** para classificação de níveis de obesidade.

## Objetivos

-   Classificar indivíduos quanto ao nível de obesidade usando KNN.
-   Otimizar hiperparâmetros do KNN com **Grid Search**.
-   Avaliar o desempenho com validação cruzada **Leave-One-Out (LOO)**.
-   Identificar possíveis riscos de overfitting.

## Metodologia

1. Pré-processamento dos dados (igual ao Trabalho 1).
2. Definição de espaço de busca para hiperparâmetros:
    - Número de vizinhos: `[1, 2, 3, 4, 5, 6, 10]`
    - Tipo de peso: `['uniform', 'distance']`
3. Uso de Grid Search com validação LOO.
4. Execução repetida 30 vezes para robustez estatística.

## Principais Resultados

-   Melhor configuração: `n_neighbors=1`, `weights='uniform'`.
-   Acurácia, F1 e recall = **1.0** em todas as execuções.
-   Alto risco de overfitting devido ao uso do LOO (modelo treinado com quase todos os dados e testado em apenas 1).

## Estrutura

-   `codigo/` – Scripts e notebooks de processamento e classificação.
-   `relatorio.pdf` – Relatório completo do trabalho.
