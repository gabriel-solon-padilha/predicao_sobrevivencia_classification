# Predição de sobrevivência desastre do titanic

## Introdução

Meu quarto projeto de machine learning em que faço o uso de modelos de classificação para predição da sobrevivência ou não no desastre do titanic. Nesse notebook busquei mudularizar melhor meu código o organizando todo em funções para melhorar a legibilidade. Além disso, foi a primeira vez que usei a biblioteca de otimização de hiperparâmetros "optuna". 

Esse notebook consiste na análise do dataset "titanic" que é composto pelas seguintes features:
- Pclass: classe que o passageiro escolher (1a,2a ou 3a)
- Name: nome do passageiro
- Sex: sexo do passageiro (masculino ou feminino)
- Age: idade dos passageiros
- SibSp: número de irmãos/cônjuges a bordo
- Parch: número de pais/filhos a bordo
- Ticket: ticket de cada passageiro
- Fare: preço do ticket pago
- Cabin: cabine de cada passageiro
- Embarked: porto que cada passageiro embarcou

A variável target é a feature "Survived" e ele tem os valores 0 (morreu) ou 1 (sobreviveu)

## Desenvolvimento

Nesse projeto passei pelas seguintes etapas:
1) Carregamento, Limpeza, Encoding e Preenchimento de missings
2) EDA
3) Feature engeneering
4) Seleção de modelo
5) Tunning de hiper parâmetros

## Resultados encontrados
Model |	accuracy	|precision	|recall	  |f1	|auc
------|-----------|-----------|---------|---|----
GradientBoosting	|0.830532	|0.819860	|0.719096	|0.764394	|0.884284
CatBoost	|0.830525	|0.825697	|0.710401	|0.761512	|0.876607
Random Forest	|0.829421	|0.801294	|0.736658	|0.766671	|0.871824
LightGBM	|0.835039	|0.798463	|0.765942	|0.779751	|0.865217
XGBoost	|0.824951	|0.784288	|0.751364	|0.766272	|0.858687
AdaBoost	|0.810363	|0.765918	|0.736701	|0.748995	|0.852855
Logistic Regression	|0.795719	|0.748464	|0.704518	|0.725014	|0.838094
Decision Tree	|0.780033	|0.717782	|0.707417	|0.710947	|0.766358
