# EDA e Modelo Preditivo para o dataset 'Bank Marketing'

Este projeto realiza uma análise exploratória de dados (EDA) e constrói um modelo preditivo para prever a probabilidade de um cliente adquirir um produto bancário.

## Objetivos do Projeto
- Realizar uma análise exploratória do dataset.
- Obter insights sobre variáveis como idade, profissão, saldo, empréstimos, entre outras.
- Construir um modelo preditivo para identificar clientes com maior probabilidade de adquirir o produto.
- Tunar hiperparâmetros do modelo e melhorar a acurácia.

## Durante a EDA, foram extraídos os seguintes insights:
- Distribuição das Colunas: A análise inicial revelou como variáveis como idade, profissão e saldo dos clientes se distribuem.
- Saldo dos Clientes: Ao analisar a distribuição dos saldos, foi possível identificar se o saldo influencia a probabilidade de aquisição do produto. Observamos que os outliers têm um impacto considerável nas decisões de negócios.
- Influência do Empréstimo: Foi observado que, entre os clientes que não tomaram empréstimos, 12,48% adquiriram o produto bancário, enquanto entre os que tomaram empréstimos, apenas 6,20% adquiriram o produto.
- Educação e Profissão: Clientes com educação 'primary' demonstraram uma taxa de conversão maior, especialmente quando são da profissão 'student' ou 'unknown'.
- Probabilidade Condicional de Empréstimo: A análise também calculou a probabilidade condicional de um cliente contratar um empréstimo com base em sua interação com a instituição bancária (se foi ou não contatado anteriormente).

## Etapas do Modelo Preditivo:
- Pré-processamento: Transformação de variáveis categóricas e normalização de algumas variáveis numéricas.
- Treinamento: O modelo foi treinado utilizando um conjunto de dados balanceado, garantindo que as classes não fossem desproporcionais.
- Tuning de hiperparâmetros: Foram ajustados hiperparâmetros como n_estimators, max_depth e min_samples_split para melhorar a performance do modelo.
- Ajuste de probabilidades: Foi feita uma modificação nas probabilidades de previsão para aumentar a sensibilidade do modelo para detectar mais casos positivos (clientes que adquirirão o produto).
