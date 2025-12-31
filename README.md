# Data Science Case: Predictive Sales Modeling (Retail)

## 📌 Executive Summary
Este projeto implementa uma solução de análise preditiva para o setor de varejo, utilizando **Regressão Linear** para modelar e projetar o faturamento mensal. O foco técnico está na transformação de dados estruturados e na validação da tendência de crescimento para suporte à tomada de decisão estratégica em Dezembro.

---

## 🏗️ Technical Architecture

O projeto foi estruturado seguindo as melhores práticas de desenvolvimento voltadas a dados:

* **Ingestão:** Processamento de dados via estruturas de dicionários Python transformados em vetores multidimensionais.
* **Modeling:** Implementação de regressão via Ordinary Least Squares (OLS) através do `scikit-learn`.
* **Evaluation:** Análise de tendência linear e projeção de variáveis independentes (time-series as features).

---

## 🛠️ Stack Tecnológica

* **Core:** Python 3.9+
* **Data Wrangling:** Pandas & NumPy
* **Machine Learning:** Scikit-Learn (LinearRegression)
* **Data Visualization:** Matplotlib (Plotagem de linha de tendência)

---

## 📊 Methodology & Feature Engineering

Para que o algoritmo de regressão linear processasse os dados temporais, foi aplicada uma transformação de variáveis categóricas ordinais:

1.  **Mapeamento Temporal:** Conversão dos meses (Jan-Dez) para um espaço vetorial discreto $[1, 12]$.
2.  **Model Fitting:** Otimização do erro quadrático médio para encontrar a melhor reta que descreve o comportamento de vendas:
    $$y = \beta_0 + \beta_1x + \epsilon$$
3.  **Inference:** Predição aplicada ao mês 12 com base nos pesos aprendidos durante o treinamento.

---

## 📈 Resultados Obtidos

* **Comportamento:** Identificou-se uma correlação linear perfeita entre o avanço dos meses e o aumento das vendas.
* **Forecast (Dezembro):** A predição apontou um faturamento de **R$ 3.300,00**, validando a escalabilidade do negócio para o período de pico.
* **Business Impact:** A precisão do modelo permite um planejamento de estoque com margem de segurança reduzida, otimizando o fluxo de caixa.

---

