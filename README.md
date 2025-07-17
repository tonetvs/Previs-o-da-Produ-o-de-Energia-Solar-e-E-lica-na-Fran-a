# Previsão da Produção de Energia Solar e Eólica na França

Este projeto desenvolve modelos preditivos para estimar a produção horária de energia solar e eólica na França. Utilizando dados históricos oficiais e enriquecimento com variáveis temporais, sazonais e estatísticas, a solução tem como objetivo apoiar o planejamento energético, melhorar a integração de fontes renováveis à rede e contribuir para uma operação mais eficiente do sistema elétrico.

## Objetivo

Antecipar a geração de energia renovável com boa acurácia e granularidade horária, utilizando técnicas de aprendizado de máquina e redes neurais recorrentes (LSTM), considerando a natureza intermitente da produção solar e eólica.

## Metodologia

1. Pré-processamento dos dados:
   - Conversão e ordenação temporal
   - Remoção de registros nulos
   - Criação de variáveis temporais (hora, dia da semana, mês)
   - Decomposição de séries com STL para separar tendência e sazonalidade

2. Modelagem preditiva:
   - LSTM (Long Short-Term Memory)
   - Random Forest Regressor
   - Stacking com Lasso e XGBoost
   - Otimização de hiperparâmetros via GridSearchCV

3. Avaliação de desempenho:
   - Métricas: MAE, RMSE, R²
   - Visualizações comparando as previsões com a produção real

## Bibliotecas Utilizadas

pandas  
numpy  
matplotlib  
seaborn  
plotly  
scikit-learn  
xgboost  
tensorflow  
statsmodels

## Execução

O notebook já contém todas as células executadas e comentadas.  
Profissionais da área podem abri-lo diretamente em qualquer ambiente compatível com Jupyter Notebook para explorar os resultados, adaptar o código ou realizar reexecuções conforme necessário.

## Estrutura

previsao-energia-renovavel/  
├── notebooks/  
│   └── Previsao_energia_solar_eolica.ipynb  
├── data/  
|── README.md  
├── requirements.txt  
└── LICENSE

## Autor

Heitor Tonet  
Engenheiro de Controle e Automação e Cientista de Dados, com foco em manutenção preditiva industrial, especializado em modelos de RUL, detecção de falhas, séries temporais e simulações baseadas em física.

## Licença

Este projeto está sob a licença MIT.
