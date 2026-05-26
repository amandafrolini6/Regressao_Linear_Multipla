# Regressão Linear Simples e Regressão Linear Múltipla

## Objetivo

Este projeto tem como objetivo comparar os modelos de Regressão Linear Simples e Regressão Linear Múltipla utilizando o dataset **kc_house_data.csv**, analisando qual deles explica melhor o preço dos imóveis com base em suas características.

## Conceitos

### Regressão Linear Simples
A Regressão Linear Simples utiliza apenas uma variável independente para prever uma variável dependente. No contexto deste projeto, o preço do imóvel é estimado a partir de apenas uma característica, como por exemplo a área da casa.

### Regressão Linear Múltipla
A Regressão Linear Múltipla utiliza duas ou mais variáveis independentes para realizar a previsão. Dessa forma, além da área, podem ser consideradas características como número de quartos, banheiros, andares, condição do imóvel e metragem do terreno.

## Metodologia

1. Importação do dataset `kc_house_data.csv`.
2. Tratamento e seleção dos dados.
3. Treinamento do modelo de Regressão Linear Simples.
4. Treinamento do modelo de Regressão Linear Múltipla.
5. Comparação dos resultados por métricas de desempenho.

## Resultados

Os resultados demonstram que a Regressão Linear Múltipla apresenta melhor capacidade de previsão dos preços dos imóveis quando comparada à Regressão Linear Simples.

Isso ocorre porque o valor de uma residência não depende apenas de uma única característica, mas da combinação de diversos fatores que influenciam diretamente seu preço de mercado.

## Conclusão

A Regressão Linear Múltipla é mais adequada para explicar e prever o preço dos imóveis do dataset analisado, pois considera simultaneamente várias características relevantes, resultando em maior precisão e melhor ajuste aos dados observados.
