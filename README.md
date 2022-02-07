# projeto_8_predicao_sobrevivencia_dataset_titanic
Meu 8 projeto em python em que faço o uso de modelos de classificação para predição da sobrevivência ou não no desastre do titanic. Nesse notebook busquei mudularizar melhor meu código o organizando todo em funções para melhorar a legibilidade. Além disso, foi a primeira vez que usei a biblioteca de otimização de hiperparâmetros "optuna". 

Esse notebook consiste na análise do dataset "titanic" que é composto pelas seguintes features:
- Pclass: classe que o passageiro escolher (1a,2a ou 3a) -> int
- Name: nome do passageiro -> string
- Sex: sexo do passageiro (masculino ou feminino) -> string
- Age: idade dos passageiros -> float
- SibSp: número de irmãos/cônjuges a bordo -> int
- Parch: número de pais/filhos a bordo -> int
- Ticket: ticket de cada passageiro -> string
- Fare: preço do ticket pago -> float
- Cabin: cabine de cada passageiro -> float
- Embarked: porto que cada passageiro embarcou -> string

A variável target é a feature "Survived" e ele tem os valores 0 (morreu) ou 1 (sobreviveu)

Nesse projeto passei pelas seguintes etapas:
1) Carregamento, Limpeza, Encoding e Preenchimento de missings
2) EDA
3) Feature engeneering
4) Seleção de modelo
5) Tunning de hiper parâmetros

