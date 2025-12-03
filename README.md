# 📊 Previsão de Estoque Inteligente na AWS com SageMaker Canvas

Bem-vindo ao projeto de Previsão de Estoque Inteligente! Neste laboratório, utilizei o poder do **Amazon SageMaker Canvas** da AWS para criar previsões de estoque baseadas em Machine Learning (ML) de forma visual, sem a necessidade de escrever código (no-code).

## 📋 Descrição do Projeto

O objetivo deste projeto foi construir um modelo preditivo capaz de estimar a demanda futura de produtos em estoque. Através de dados históricos, treinei um modelo de *Time Series Forecasting* (Previsão de Séries Temporais) para auxiliar em um planejamento logístico mais eficiente.

## 🚀 Tecnologias Utilizadas

* **Amazon AWS:** Plataforma de computação em nuvem.
* **Amazon SageMaker Canvas:** Ferramenta visual (*no-code*) para construção e implantação de modelos de ML.
* **Dataset:** Arquivo CSV contendo histórico de vendas e estoque de produtos.

---

## 🛠️ Passo a Passo do Projeto

Abaixo descrevo o fluxo de trabalho completo realizado dentro da interface do SageMaker Canvas.

### 1. Importação e Preparação dos Dados
O primeiro passo foi carregar o dataset (arquivo CSV) para dentro do SageMaker Canvas. O dataset continha informações cruciais como identificador do produto, datas das transações e a quantidade em estoque.

Após a importação, foi realizada uma rápida visualização para garantir que os tipos de dados (numéricos, datas) foram identificados corretamente pela ferramenta.

### 2. Construção do Modelo (Build)
Na etapa de construção, configurei o Canvas para um problema de Séries Temporais:

* **Coluna Alvo (Target):** Defini a coluna que representa a quantidade de estoque a ser prevista.
* **Coluna de Identificação (Item ID):** Configurei o ID único de cada produto.
* **Coluna de Tempo (Timestamp):** Apontei a coluna contendo as datas dos registros.

Utilizei a função **"Quick Build"** (Construção Rápida) para que o Canvas selecionasse e treinasse automaticamente o melhor algoritmo para os dados.

### 3. Análise de Resultados (Analyze)
Após o treinamento, o Canvas apresentou as métricas de performance do modelo.

**[INSIRA UM PRINT AQUI DA TELA "ANALYZE" MOSTRANDO OS GRÁFICOS DE ACURÁCIA E AS MÉTRICAS (WAPE, RMSE)]**

*A análise dos gráficos demonstrou a capacidade do modelo em acompanhar a sazonalidade e as tendências de venda dos produtos principais.*

### 4. Geração de Previsões (Predict)
Com o modelo validado, a etapa final foi gerar previsões. O SageMaker Canvas permite simular cenários hipotéticos (alterando preços, por exemplo) ou gerar previsões em lote para datas futuras.

**[INSIRA UM PRINT AQUI DA TELA "PREDICT" MOSTRANDO UMA LINHA DO TEMPO COM A PREVISÃO FUTURA DO ESTOQUE]**

---

## 📊 Conclusões

Este projeto demonstrou como ferramentas *no-code* como o Amazon SageMaker Canvas democratizam o acesso à Inteligência Artificial. Foi possível sair de um arquivo CSV bruto para um modelo de previsão de estoque funcional em poucos passos, permitindo que o foco permaneça na estratégia de negócios e não na complexidade da codificação.

---
**Autor:** [Seu Nome Aqui]
