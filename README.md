# Detecção de Fraudes em Transações de Cartão de Crédito

Projeto de Ciência de Dados e Machine Learning para identificar transações fraudulentas em um dataset real e altamente desbalanceado de cartões de crédito (transações europeias, setembro de 2013 — Kaggle / ULB Machine Learning Group).

## 🎯 Objetivo

Construir e comparar diferentes modelos de classificação capazes de distinguir transações normais de transações fraudulentas, com foco nas métricas corretas para problemas desbalanceados (recall, precisão e F1-score) e na explicabilidade do modelo final.

## 🧠 O que foi feito

- Análise exploratória e identificação do forte desbalanceamento das classes (~0,17% de fraudes)
- Engenharia de atributos (transformação logarítmica e padronização do valor da transação)
- Separação estratificada entre treino e teste
- Treinamento e avaliação de 3 modelos: **Regressão Logística**, **Random Forest** e **XGBoost**
- Comparação entre **undersampling** e **oversampling** para lidar com o desbalanceamento
- Construção de um **Pipeline** e ajuste de **threshold** de decisão
- Otimização de hiperparâmetros com **GridSearchCV** (foco em recall)
- Explicabilidade do modelo com **SHAP**
- Comparação final entre todos os modelos testados

## 🛠️ Tecnologias

Python · pandas · numpy · scikit-learn · XGBoost · imbalanced-learn · SHAP · matplotlib · seaborn

## ▶️ Como executar

```bash
pip install -r requirements.txt
jupyter notebook deteccao_fraude_cartao_credito.ipynb
```

## 📊 Dataset

[Credit Card Fraud Detection — Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

## 📌 Status

Projeto desenvolvido como parte da trilha de Análise de Dados / Detecção de Anomalias da DIO, com testes e conclusões próprias.
