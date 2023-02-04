# [Lighthouse] Desafio Cientista de Dados - Manutenção preventiva

Os problemas de classificação são aqueles onde se busca encontrar uma classe, dentro das possibilidades limitadas existentes. Esta classe pode ser se um aluno foi aprovado ou reprovado, se uma pessoa possui uma doença ou não, dentre outras tantas possibilidades, sendo que nestes casos ou a previsão será uma ou outra

O objetivo deste trabalho é identificar, atravéis de uma modelo de calssificação, quais máquinas apresentam potencial de falha tendo como base dados extraídos através de sensores durante o processo de manufatura.

## Analisando os Dados

Para entender como os dados estavam compostos, foi feito uma analise estatistica usando o describe() mostando alguns parametros importantes do conjunto de dados.

Foi feita uma normalização dos dados para mudar os valores das colunas numéricas no conjunto de dados e passar para uma escala comum, sem distorcer as diferenças nos intervalos de valores nem perder informações.

Analisando a distribuição da variável alvo, pode ser observado que os dados estvam desbalanceados. Para corrigir esse problema foi feito um balanceamento utilizando a classe SMOTE da biblioteca imbalanced-learn.

## Modelagem

O algoritmo Random Forest é um algoritmo de aprendizado de máquina utilizado para realizar predições. Resumidamente, o algoritmo cria de forma aleatória várias Árvores de Decisão (Decision Trees) e combina o resultado de todas elas para chegar no resultado final.

O RandomForestClassifier cria um conjunto de árvores de decisão a partir de um subconjunto selecionado aleatoriamente do conjunto de treinamento. É basicamente um conjunto de árvores de decisão de um subconjunto selecionado aleatoriamente do conjunto de treinamento e, em seguida, coleta os votos de diferentes árvores de decisão para decidir a previsão final.

O aprendizado supervisionado ocorre quando o modelo aprende a partir de resultados pré-definidos, utilizando os valores passados da variável target para aprender quais devem ser seus resultados de saída. Estes mesmos valores servem como “supervisão” destas previsões, permitindo o ajuste nas previsões com base nos erros.



### 📋 Pré-requisitos

imblearn==0.0
pandas==1.5.3
python==3.9.12
numpy==1.21.5
sklearn==1.2.1
matplotlib==3.5.1

