# Desafio-ONE---Data-Science---TelecomX-Etapa-2


## Tecnologia

Os softwares utilizados neste projeto foram:

* Jupyter Anaconda
* Python


## Serviço usado:

* Github


## Bibliotecas Python

* Pandas
* matplotlib
* sklearn


* ## Descrição do Projeto </h1>

Este projeto é a continuação do desafio de Data Science, focado na previsão de churn (evasão de clientes) da empresa de telecomunicações fictícia TelecomX. Após a análise exploratória na Etapa 1.

link do repositório da primeira etapa: https://github.com/bonfimdoprado/Challenge-ONE-Data-Science---TelecomX

A Etapa 2 se concentrou na construção, treinamento e avaliação de um modelo de Regressão Logística para prever a probabilidade de um cliente evadir. O objetivo final é fornecer uma ferramenta preditiva para ajudar a equipe de negócio a tomar decisões mais estratégicas de retenção de clientes.


### 1. Pré-processamento e Transformação de Dados

Antes de construir o modelo, os dados foram preparados para serem utilizados pelo algoritmo de Machine Learning. As etapas de pré-processamento e transformação incluíram:

- Limpeza de Dados: Valores ausentes foram tratados e a coluna Charges.Total foi transformada para o tipo numérico.

- Categorização: As colunas Charges.Monthly, Charges.Total e tenure foram agrupadas em categorias (ex: "Low", "Medium") com base nos seus quartis para facilitar a análise e a modelagem.

- One-Hot Encoding: As variáveis categóricas (como gender, Contract, PaymentMethod e as novas colunas de grupo) foram transformadas em formato numérico. O One-Hot Encoding cria novas colunas binárias para cada categoria, permitindo que o modelo as processe sem atribuir uma ordem de importância incorreta.

 <img width="914" height="630" alt="Image" src="https://github.com/user-attachments/assets/8fb9eae2-a6b4-450b-ac2b-bdd99a2da2b4" />


### 2. Análise e Avaliação do Modelo de Regressão Logística

A modelagem de Regressão Logística foi construída seguindo as etapas de pré-processamento, divisão de dados e treinamento do modelo. Os resultados obtidos demonstram o bom desempenho do modelo na tarefa de prever a evasão, conforme as métricas abaixo.

Acurácia e ROC AUC
A acurácia do modelo foi de 81%, o que significa que ele acertou a previsão em 81 de cada 100 casos.

No entanto, a métrica mais relevante para este problema é a área sob a curva ROC (ROC AUC). Com um ROC AUC Score de 0.85, o modelo se mostra excelente na sua capacidade de distinguir entre clientes que irão evadir (Churn) e aqueles que permanecerão, sendo significativamente melhor que uma previsão aleatória.




 Análise e Avaliação do Modelo de Regressão Logística
A modelagem de Regressão Logística foi construída seguindo as etapas de pré-processamento, divisão de dados e treinamento do modelo. Os resultados obtidos demonstram o bom desempenho do modelo na tarefa de prever a evasão, conforme as métricas abaixo.

Acurácia e ROC AUC
A acurácia do modelo foi de 81%, o que significa que ele acertou a previsão em 81 de cada 100 casos.

No entanto, a métrica mais relevante para este problema é a área sob a curva ROC (ROC AUC). Com um ROC AUC Score de 0.85, o modelo se mostra excelente na sua capacidade de distinguir entre clientes que irão evadir (Churn) e aqueles que permanecerão, sendo 

