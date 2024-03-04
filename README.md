# Estudo do Algoritmo de Naive Bayes

Este é um projeto de estudo focado na implementação e análise do algoritmo de Naive Bayes para classificação de dados. Utilizamos duas bases de dados diferentes para explorar o desempenho do modelo em contextos distintos.

## Base de Dados de Crédito

A primeira base de dados é sobre risco de crédito, adaptada da fonte [Kaggle](https://www.kaggle.com/laotse/credit-risk-dataset). Ela consiste em informações sobre clientes, como renda anual, idade, valor do empréstimo e se o empréstimo foi pago ou não. O atributo alvo é binário, onde 0 indica que o empréstimo foi pago e 1 indica que não foi pago.

## Base de Dados do Censo

A segunda base de dados é sobre informações do censo, obtida a partir do [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/adult). Esta base contém diversas características demográficas e sociais dos indivíduos, como idade, educação, estado civil, entre outros. O objetivo é prever se um indivíduo possui renda superior a $50,000 por ano, com o atributo alvo sendo binário também.

## Preprocessamento dos Dados

Para preparar os dados para o modelo de Naive Bayes, realizamos várias etapas de preprocessamento, incluindo:

- Divisão dos dados em previsores e classe.
- Tratamento de atributos categóricos utilizando LabelEncoder e OneHotEncoder.
- Escalonamento dos valores para uma melhor convergência do modelo.

## Divisão entre Conjuntos de Treinamento e Teste

Utilizamos a função `train_test_split` da biblioteca `scikit-learn` para dividir os dados em conjuntos de treinamento e teste. Isso nos permite avaliar o desempenho do modelo em dados não vistos durante o treinamento.

## Implementação do Naive Bayes

Para a implementação do algoritmo de Naive Bayes, utilizamos a classe `GaussianNB` da biblioteca `scikit-learn`, adequada para variáveis contínuas.

## Resultados

Após treinar o modelo de Naive Bayes nas duas bases de dados, obtivemos os seguintes resultados de acurácia na classificação:

- **Base de Dados de Crédito**: 93.80%
- **Base de Dados do Censo**: 47.67%

Esses resultados nos fornecem insights sobre a eficácia do algoritmo de Naive Bayes em diferentes contextos e a qualidade dos dados utilizados.
