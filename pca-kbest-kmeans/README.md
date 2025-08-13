# Trabalho 1 – Redução de Dimensionalidade e Agrupamento (PCA, SelectKBest e K-Means)

Este trabalho realiza uma análise exploratória e de agrupamento utilizando o dataset de níveis de obesidade.

## Objetivos

-   Analisar estatísticas descritivas (média, desvio padrão, variância, correlação).
-   Reduzir dimensionalidade com **PCA (Principal Component Analysis)**.
-   Selecionar as melhores características com **SelectKBest**.
-   Agrupar os dados com **K-Means**.
-   Avaliar a qualidade dos clusters com **Davies-Bouldin Index**.

## Metodologia

1. Pré-processamento: remoção de duplicatas, outliers e transformação de variáveis qualitativas em quantitativas.
2. Aplicação do PCA para extrair componentes principais.
3. Uso do SelectKBest para selecionar as 3 variáveis mais relevantes.
4. Treinamento do modelo K-Means em dados completos e reduzidos.
5. Avaliação dos clusters pelo índice Davies-Bouldin.

## Principais Resultados

-   O conjunto de dados reduzido obteve melhor índice Davies-Bouldin que o conjunto completo.
-   A redução de dimensionalidade melhorou a performance de agrupamento.

## Estrutura

-   `codigo/` – Scripts e notebooks de processamento e análise.
-   `relatorio.pdf` – Relatório completo do trabalho.
