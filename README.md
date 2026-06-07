# 🏠 Previsão de Preço de Casas - Melbourne

[![Python 3.8+](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.2-orange.svg)](https://scikit-learn.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 📌 Sobre o Projeto

Este projeto implementa um modelo de **Regressão Linear** para prever o preço de casas em Melbourne (Austrália) utilizando apenas o número de quartos como variável preditora. O objetivo é entender o fluxo básico de um projeto de Machine Learning e avaliar a qualidade de um modelo simples.

**Dataset:** Melbourne Housing Snapshot (Kaggle/UCI)

## 🎯 Objetivos

- Implementar o primeiro modelo de ML (Regressão Linear)
- Analisar o impacto da divisão treino/teste nos resultados
- Calcular e interpretar métricas de avaliação (R², RMSE, MAE)
- Visualizar a relação entre variáveis

## 📊 Principais Resultados

| Proporção (Teste) | R²     | Coeficiente (preço por quarto) |
|-------------------|--------|-------------------------------|
| 10%               | 0.2517 | R$ 330.611                     |
| 20%               | 0.2556 | R$ 331.068                     |
| 30%               | 0.2430 | R$ 330.004                     |
| 40%               | 0.2439 | R$ 328.895                     |

### Modelo Final (80% treino / 20% teste)
📊 MÉTRICAS:
- R²: 0.2556
- RMSE: 543.758,74 AUD
- MAE: 384.558,01 AUD

📈 EQUAÇÃO DA RETA:
- Preço = 331.067,71 × Quartos + 102.941,12

## 🔍 Interpretação dos Resultados

- O R² de **0.2556** significa que apenas **25,6%** da variação do preço é explicada pelo número de quartos
- Os outros **74,4%** dependem de outros fatores (localização, tamanho, ano, etc.)
- A divisão treino/teste mostrou que o modelo é relativamente estável, com R² variando entre 0.24 e 0.26

## 🛠️ Tecnologias Utilizadas

- Python 3.8+
- Pandas (manipulação de dados)
- NumPy (operações numéricas)
- Matplotlib & Seaborn (visualizações)
- Scikit-learn (modelagem e métricas)

## 🚀 Como Executar

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/projeto-preco-casas.git
cd projeto-preco-casas ` ``` `

2. Instale as dependências:
pip install -r requirements.txt

3. Execute o Jupyter Notebook:
jupyter notebook analise_preco_casas.ipynb

## Aprendizados
- Modelos com poucas variáveis têm poder preditivo limitado
- A divisão treino/teste é essencial para evitar overfitting
- O R² sozinho não conta toda a história - é importante analisar outras métricas
- Para melhorar o modelo, seriam necessárias mais features (localização, tamanho, ano de construção)

## 📈 Próximos Passos
- Adicionar mais variáveis (tamanho do terreno, número de banheiros, localização)
- Testar outros modelos (Random Forest, XGBoost)
- Realizar feature engineering
- Aplicar validação cruzada

## 📚 Referências
- Dataset - Melbourne Housing
- Scikit-learn Documentation

## 👨‍💻 Autor
Kailayni Rodrigues Janez - @KailayniJanez
