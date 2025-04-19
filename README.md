# 🌍 Projeto Final – Pipeline de Dados com Airflow, Hadoop e Machine Learning

Este projeto implementa um pipeline completo de dados sísmicos da API USGS, com orquestração no Apache Airflow, armazenamento no HDFS (Hadoop), análise exploratória e modelagem preditiva com scikit-learn.

## 🔁 Pipeline

1. **ETL com Python**: coleta de dados da API USGS (últimos 5 anos)
2. **Orquestração**: DAG diária com Airflow
3. **Armazenamento**: Hadoop HDFS
4. **Análise**: Jupyter Notebook com visualizações e insights
5. **ML**: modelo Random Forest para prever severidade de terremotos

## 📂 Estrutura

- `dags/` – DAG Airflow
- `scripts/` – Scripts de ETL, integração com Hadoop e modelo salvo
- `notebooks/` – Análise exploratória e modelagem
- `dados/` – Arquivos .csv (ou deixe vazio e cite o HDFS)

## 🧠 Modelo

- **Tipo**: Classificação binária (severo ou não)
- **Algoritmo**: RandomForestClassifier
- **Atributos**: profundidade, latitude, longitude
- **Métrica**: F1-score, matriz de confusão, precisão

## ⚙️ Requisitos

- Python 3.10+
- Apache Airflow
- Hadoop HDFS
- scikit-learn, pandas, seaborn, matplotlib
