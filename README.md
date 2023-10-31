# Regressao_Linear.CarsPrice

## Descrição Projeto


**Conjunto de dados:** Base de dados com preços de automóveis. 


**Arquivo:** .csv


**Objetivo:** Analisar uma base de dados com preços de automóveis, aplicar machine learning com o modelo Linear Regression, a fim de prever os preços dos automóveis através das variáveis explicativas que constam na base de dados.

Regressão Linear: técnica estatística que permite modelar a relação entre variáveis independentes e uma variável dependente. 


**IDE:** Colab


**Linguagem:** Python


**Principais bibliotecas utilizadas:**

• Pandas, para manipulação e tratamento dos dados; 

• Numpy, para realizar cálculos numéricos; 

• Seaborn, para criação e visualização de gráficos interativos; 

• Sklearn, para aprendizado de machine learning.


**Modelo Utilizado:**

• Linear Regression, algoritmo de aprendizado de máquina com métodos destinados a regressão, nos quais se espera que o valor alvo seja uma combinação linear dos recursos. 

**Métricas Aplicadas:**
Aplicou-se as seguintes métricas para se avaliar a qualidade do ajuste do modelo de Regressão Linear:

• Coeficiente de Determinação - R²:  métrica estatística que varia de 0 a 1 e é usada para avaliar a qualidade do ajuste de um modelo de regressão linear. Mede a proporção da variância na variável dependente que é explicada pela variável independente. Quanto mais próximo de 1, melhor será o ajuste do modelo aos dados.

• Erro Absoluto Médio – MAE: É a média das diferenças absolutas entre as previsões e os valores reais. Ele mede o tamanho médio do erro em unidades da variável dependente.

• Erro Quadrático Médio - MSE:  É a média dos erros ao quadrado. Ele mede o tamanho médio do erro em unidades da variável dependente, mas penaliza erros maiores mais fortemente do que erros menores.

• Raiz do Erro Quadrático Médio - RMSE:  É a raiz quadrada da média dos erros ao quadrado. Ele mede o tamanho médio do erro em unidades da variável dependente, mas penaliza erros maiores mais fortemente do que erros menores .


**Sequência de processos:**

1° Instalação bibliotecas;

2° Pré-processamento de conjuntos de dados;

3° Aplicado LabelEncoder para alterar variáveis descritivas em variáveis numéricas;

4° Utilizar histograma para verificar a distribuição dos dados relacionados a variável dependente.

5° Aplicar MinMaxScaler para colocar os dados na mesma escala, ou em escalas mais próximas;

6° Aplicar Statsmodel para analisar P-Values das variáveis explicativas. Retirar do modelo variáveis com P-Values altos, testando o modelo de machine learning apenas com variáveis que possuírem P-Values abaixo de 0,05:


•	 O p-value: Em um modelo de regressão linear, o p-value é usado para testar a hipótese nula de que o coeficiente de regressão é igual a zero . Se o p-value for menor que um determinado nível de significância (geralmente 0,05), podemos rejeitar a hipótese nula e concluir que há evidências suficientes para suportar a hipótese alternativa .


7° Distribuir os dados em X (variáveis independentes) e y (variável dependente);

8° Separar base de dados para treino e teste;

9° Aplicar o método .fit do modelo de machine learning na base de treino;

10° Aplicado métrica R² na minha base de treino;

11° Aplicar o método .predict do modelo de machine learning na base de treino, para previsão;

12° Aplicado métricas MAE, MSE e RMSE na minha base predita de treino;

13° Aplicar o método .fit do modelo de machine learning na base de teste;

14° Aplicar o método .predict do modelo de machine learning na base de teste, para previsão;

15° Aplicado métricas MAE, MSE e RMSE na minha base predita de teste;


**Resultado:** O resultado da métrica aplicada no algoritmo foi de r² = 0,82. Esse resultado indica que quando minhas variáveis explicativas (independentes) mudarem, terei 82% de chance da minha variável target (dependente) mudar também. Posso dizer então que, aplicando esse modelo à essa base de dados tenho uma boa linearidade nos meus dados, conseguindo predizer bem meus resultados.

