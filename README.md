# Classificação de Objetos Astronômicos

## Modelos: 
 
### Random Forest

O Random Forest é um modelo baseado em múltiplas árvores de decisão que usa a técnica de Bagging (Bootstrap Aggregating). Ele treina várias árvores de forma independente em subconjuntos aleatórios dos dados e combina suas previsões (média para regressão, votação para classificação). Isso reduz overfitting e melhora a estabilidade do modelo.

### XGBoost
O XGBoost (Extreme Gradient Boosting) é uma versão otimizada do Gradient Boosting, projetada para alta eficiência e desempenho. Ele constrói árvores sequencialmente, corrigindo os erros da anterior, e usa técnicas como regularização L1/L2 e poda de árvores para evitar overfitting. Seu paralelismo e otimizações tornam-no muito eficiente em grandes datasets.

### LGBM 
O LightGBM (Light Gradient Boosting Machine) é uma alternativa ao XGBoost, mas com foco em maior velocidade e eficiência. Ele utiliza a técnica Histogram-based Learning, onde os dados são agrupados em bins antes do treinamento, acelerando a construção das árvores e reduzindo o uso de memória. É ideal para grandes volumes de dados.

### CatBoost 
O CatBoost é uma versão do Gradient Boosting desenvolvida pela Yandex, com melhorias no tratamento de variáveis categóricas. Ele usa técnicas como Ordered Boosting, que evita overfitting ao ordenar os dados de forma específica, e permite capturar melhor interdependências entre variáveis sem necessidade de pré-processamento complexo.


O **objetivo** deste projeto é a classificação de objetos celestes em estrelas, galáxias ou quasares utilizando diferentes modelos de
classificação supervisionados e métricas de avaliação. 

## Dependências
- ```pandas```: para leitura e manipulação dos dados
- ```numpy```: para realizar operações em array
- ```matplotlib```: para visualizações estáticas ou interativas
- ```seaborn```: para criar gráficos de forma eficiente e visualmente atraente
- ```sklearn```: para criar, treinar e implementar modelos de aprendizado de máquina

## Estrutura do projeto
1. Introdução
2. Contexto do dataset

   2.1 Por que esses estudos são importantes?

3. Dados
4. Objetivo do estudo 
5. Importação de bibliotecas
6. Coleta e exploração dos dados
7. Pré-processamento dos dados
8. Modelos de aprendizado de máquina
9. Otimização de hiperpâmetros
10. Avaliação do modelo otimizado
11. Conclusão
