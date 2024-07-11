# 📊 Previsão de Estoque Inteligente na AWS com SageMaker Canvas

Bem-vindo ao repositório do projeto "Previsão de Estoque Inteligente na AWS com SageMaker Canvas". Este projeto foi desenvolvido como parte do desafio de projeto da DIO, onde utilizei o SageMaker Canvas para criar previsões de estoque baseadas em Machine Learning (ML).

## 📋 Pré-requisitos
Antes de começar, certifique-se de ter uma conta na AWS. Se precisar de ajuda para criar sua conta, confira o repositório [AWS Cloud Quickstart](https://github.com/digitalinnovationone/lab-aws-cloud-quickstart).

## 🎯 Objetivos Deste Desafio de Projeto (Lab)
O objetivo deste projeto é desenvolver um modelo de Machine Learning para previsão de estoque utilizando o Amazon SageMaker Canvas. Através deste desafio, foram aprimoradas habilidades em ML no-code.

## 🚀 Passo a Passo

### 1. Selecionar Dataset
- A pasta `datasets` deste repositório contém os datasets utilizados para treinar e testar o modelo de ML.
- O dataset escolhido para treinar o modelo de previsão de estoque foi `canvas-sample-retail-electronics-forecast.csv`, que contém dados históricos de vendas e estoque.

### 2. Construir/Treinar
- No SageMaker Canvas, importei o dataset `canvas-sample-retail-electronics-forecast.csv`.
- Configurei as variáveis de entrada e saída de acordo com os dados:
  - A coluna alvo (target) foi `demand`.
  - Outras colunas incluídas foram `time_stamp` (timestamp), `Product_category` (text), `price` (numérico), `Location` (text) e `item_id` (text).
- O SageMaker Canvas automaticamente recomendou o tipo de modelo adequado como previsão de séries temporais (Time series forecasting).
- Iniciei o treinamento do modelo. O tempo de treinamento demorou alguns minutos.

### 3. Analisar
- Após o treinamento, examinei as métricas de performance do modelo.
- Verifiquei as principais características que influenciam as previsões.
- Fiz ajustes no modelo conforme necessário e re-treinei até obter um desempenho satisfatório.

### 4. Prever
- Usei o modelo treinado para fazer previsões de estoque.
- Exportei os resultados e analisei as previsões geradas.
- Documentei as conclusões e qualquer insight obtido a partir das previsões.

## 📈 Resultados
O modelo foi capaz de prever com precisão a quantidade de estoque necessária para os dias seguintes, considerando fatores como histórico de vendas e promoções. Isso pode ajudar a otimizar o gerenciamento de estoque, evitando excessos ou faltas de produtos.

### 📂 Estrutura do Repositório

- `datasets/`: Contém datasets para treinar o modelo.
- `README.md`: Este arquivo que você está lendo, descrevendo o projeto e os passos realizados.

Obrigado por conferir este projeto!
