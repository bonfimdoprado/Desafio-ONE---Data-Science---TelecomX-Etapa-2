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

<img width="442" height="272" alt="Image" src="https://github.com/user-attachments/assets/5be07e2a-cc5b-4da4-89bd-2057210349f1" />


### 3. Análise aprofundada das Previsões
Para entender melhor como o modelo está fazendo suas previsões, analisamos a Matriz de Confusão e a Curva ROC.

Matriz de Confusão:

- Verdadeiros Positivos (191): Clientes que evadiriam e foram identificados corretamente pelo modelo. Este é um acerto valioso, que permite à empresa atuar proativamente.

- Falsos Negativos (183): Clientes que evadiriam, mas que o modelo classificou incorretamente como 'não-churn'. Esse é o erro mais crítico, pois representa clientes perdidos que não foram identificados.

- O recall do modelo para a classe de evasão foi de aproximadamente 0.51, o que indica que ele identificou corretamente apenas cerca de metade dos clientes que de fato iriam evadir.


<img width="624" height="488" alt="Image" src="https://github.com/user-attachments/assets/b244ee84-a4a8-458f-9f11-41ae2ed7ce26" />

Curva ROC e AUC Score:

- A área sob a curva ROC (AUC) foi de 0.85. Este valor excelente indica que o modelo tem uma alta capacidade de distinguir entre clientes que irão evadir (churn) e aqueles que permanecerão, sendo significativamente melhor que uma previsão aleatória.

<img width="612" height="445" alt="Image" src="https://github.com/user-attachments/assets/1e225bfd-3d92-428c-a145-5bc84868b104" />


### 4. Resumo do projeto

O projeto de Análise e Previsão de Churn para a TelecomX foi dividido em duas etapas principais.

1. Análise Exploratória e de Fatores (Etapa 1): Identificamos os principais fatores que influenciam a evasão de clientes, como o tipo de pagamento, o contrato e a idade (clientes idosos). Essa análise inicial forneceu insights valiosos para a empresa.

2. Modelagem Preditiva (Etapa 2): Com base nos insights da primeira etapa, criamos e avaliamos um modelo de Regressão Logística. Após o pré-processamento de dados e a categorização de variáveis-chave, o modelo obteve uma acurácia de 81%. Mais importante, o ROC AUC Score de 0.85 demonstra a sua excelente capacidade de prever com precisão os clientes que estão em risco de evadir. A Matriz de Confusão revelou que o modelo identificou corretamente a maioria dos clientes que não evadiram, mas que ainda tem espaço para melhoria na identificação dos que de fato evadirão.

O recall do modelo de 0.51 mostra que apenas pouco mais da metade dos clientes que de fato evadiriam foram identificados. Esse é um índice que precisa de atenção, pois afeta diretamente a capacidade da empresa de atuar proativamente na retenção de clientes.

Em suma, o projeto resultou em uma ferramenta poderosa para a TelecomX, que pode ser usada para identificar clientes em risco de churn de forma proativa. O modelo oferece uma base sólida para a criação de estratégias de retenção de clientes mais eficazes e direcionadas. A ideia no futuro é continuar melhorando a previsibilidade do modelo com técnicas mais avançadas para melhorar este índice, mas já foi muito importante entender todo o processo de pré-processamento e machine learning.

## Autor

* **Matheus Bonfim do Prado**: @bonfimdoprado (https://github.com/bonfimdoprado)
