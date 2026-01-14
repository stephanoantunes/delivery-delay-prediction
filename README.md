# Predição de Atrasos em Entregas no E-commerce

## Visão Geral
Atrasos em entregas impactam diretamente a satisfação do cliente e aumentam custos
operacionais em operações de e-commerce.  
Este projeto tem como objetivo analisar dados históricos de pedidos e desenvolver
um modelo de machine learning capaz de prever o risco de atraso na entrega.

O foco é demonstrar um fluxo completo de Ciência de Dados, desde a análise exploratória
até a modelagem preditiva.

---

## Dataset
Foi utilizado o **Brazilian E-Commerce Public Dataset (Olist)**, que contém informações
reais de um marketplace brasileiro, incluindo datas de compra, envio, entrega,
localização do cliente e avaliações.

---

## Estrutura do Projeto

delivery-delay-prediction/
│
├── data/
│ ├── raw/ # Dados originais
│ └── processed/ # Dataset tratado para modelagem
│
├── notebooks/
│ ├── 01_eda.ipynb
│ ├── 02_feature_engineering.ipynb
│ └── 03_modeling.ipynb
│
├── README.md
└── requirements.txt


---

## Metodologia

### 1. Análise Exploratória (EDA)
- Criação da variável alvo (`entrega_atrasada`)
- Análise da taxa de atraso por estado
- Avaliação do impacto do atraso na nota do cliente

### 2. Feature Engineering
- Criação de variáveis temporais
- Extração de informações de calendário
- Tratamento de variáveis categóricas com one-hot encoding

### 3. Modelagem Preditiva
- Modelo baseline: Regressão Logística
- Modelo final: Random Forest
- Avaliação com Precision, Recall, F1-score e ROC-AUC

---

## Resultados
O modelo Random Forest apresentou desempenho superior ao baseline, com melhor capacidade
de identificar pedidos com risco de atraso. As variáveis relacionadas ao tempo de entrega
foram as mais relevantes para a predição.

---

## Conclusão
O modelo desenvolvido pode ser utilizado como apoio à tomada de decisão logística,
permitindo ações preventivas, como priorização de pedidos críticos ou comunicação
antecipada com o cliente.

---

## Tecnologias Utilizadas
- Python
- Pandas, NumPy
- Scikit-learn
- JupyterLab (Anaconda)

---

## Autor
Stephano Douglas Antunes
Projeto desenvolvido para fins de portfólio em Ciência de Dados.