# 🏠 Precificação Inteligente de Imóveis (House Prices Advanced Regression)

## 📋 Sobre o Projeto
Modelo preditivo desenvolvido para estimar preços de venda de imóveis residenciais em Ames, Iowa. O projeto simula um desafio real de uma PropTech, utilizando técnicas avançadas de Engenharia de Atributos e Modelos de Ensemble.

**Dataset:** [House Prices - Advanced Regression Techniques (Kaggle)](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)

## 🛠 Tecnologias Utilizadas
*   **Python 3.x**
*   **Pandas & Numpy:** Manipulação e limpeza de dados.
*   **Seaborn & Matplotlib:** Análise exploratória visual.
*   **Scikit-Learn:** Pré-processamento, Lasso Regression e Validação Cruzada.
*   **XGBoost:** Gradient Boosting para captura de padrões não-lineares.

## ⚙️ Principais Etapas
1.  **EDA (Análise Exploratória):** Correção de assimetria (`log1p`) na variável alvo.
2.  **Limpeza de Dados:** Tratamento de valores nulos com distinção semântica entre "Zero" e "Inexistente".
3.  **Feature Engineering:**
    *   Criação da variável `TotalSF` (Área Total Construída).
    *   Tratamento de outliers bivariados.
4.  **Modelagem:**
    *   Criação de Pipeline com `RobustScaler`.
    *   Ensemble: Lasso (70%) + XGBoost (30%).

## 📊 Resultados
O modelo atingiu um **RMSLE (Root Mean Squared Logarithmic Error) de ~0.1119** na validação cruzada, demonstrando alta capacidade de generalização.

## 🚀 Como Executar
1. Clone este repositório.
2. Instale as dependências: `pip install pandas numpy seaborn scikit-learn xgboost`.
3. Execute o notebook `01_analise_exploratoria.ipynb`.

---
*Desenvolvido durante Mentoria de Machine Learning Prático.*
