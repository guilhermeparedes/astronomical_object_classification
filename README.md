# Classificação de Objetos Astronômicos


## Objetivo

O **objetivo** deste projeto é a classificação de objetos celestes em estrelas, galáxias ou quasares utilizando diferentes modelos de
classificação supervisionados e métricas de avaliação. 


## Modelos
 
### Random Forest

O Random Forest é um modelo baseado em múltiplas árvores de decisão que usa a técnica de Bagging (Bootstrap Aggregating). Ele treina várias árvores de forma independente em subconjuntos aleatórios dos dados e combina suas previsões (média para regressão, votação para classificação). Isso reduz overfitting e melhora a estabilidade do modelo.

### XGBoost
O XGBoost (Extreme Gradient Boosting) é uma versão otimizada do Gradient Boosting, projetada para alta eficiência e desempenho. Ele constrói árvores sequencialmente, corrigindo os erros da anterior, e usa técnicas como regularização L1/L2 e poda de árvores para evitar overfitting. Seu paralelismo e otimizações tornam-no muito eficiente em grandes datasets.

### LGBM 
O LightGBM (Light Gradient Boosting Machine) é uma alternativa ao XGBoost, mas com foco em maior velocidade e eficiência. Ele utiliza a técnica Histogram-based Learning, onde os dados são agrupados em bins antes do treinamento, acelerando a construção das árvores e reduzindo o uso de memória. É ideal para grandes volumes de dados.

### CatBoost 
O CatBoost é uma versão do Gradient Boosting desenvolvida pela Yandex, com melhorias no tratamento de variáveis categóricas. Ele usa técnicas como Ordered Boosting, que evita overfitting ao ordenar os dados de forma específica, e permite capturar melhor interdependências entre variáveis sem necessidade de pré-processamento complexo.


## Dependências
- ```pandas```: para leitura e manipulação dos dados
- ```numpy```: para realizar operações em array
- ```matplotlib```: para visualizações estáticas ou interativas
- ```seaborn```: para criar gráficos de forma eficiente e visualmente atraente
- ```sklearn```: para criar, treinar e implementar modelos de aprendizado de máquina

## Estrutura do projeto

- **1. Introdução**
- **2. Motivação e Contexto do DataSet**
  - Importância do Estudo?
- **3. Dados**
  - Atributo alvo: Classe
    - Classes do Problema: Estrelas, Galáxias e Quasares
  - Atributos Físicos
    - Filtros Fotométricos
    - Redshift
    - Coordenadas Alpha e Delta
- **4. Objetivo do Estudo**
- **5. Importação de Bibliotecas e Pacotes**
- **6. Análise Exploratória de Dados (EDA)**
  - Carregamento e Visualização dos Dados
  - Análise Descritiva
  - Visualização dos Dados
    - Distribuição das Classes
  - Análise de Correlação
    - Correlação de Pearson
    - Verificação de Atributos Idênticos
    - Informação Mútua
    - Correlação Entre Coordenadas Equatoriais e a Variável Alvo
    - Correlação Entre Redshift e a Variável Alvo
  - Identificação de Outliers
- **7. Pré-processamento dos Dados**
  - Seleção de Atributos
  - Transformação dos Dados
  - Redução de Dimensionalidade
  - Codificação de Variáveis Categóricas
  - Divisão dos Dados
  - Balanceamento dos Dados
    - Oversampling
    - Undersampling
- **8. Aprendizado de Máquina**
  - Modelos de Aprendizado de Máquina
    - Random Forest
    - XGBoost
    - LightGBM
    - CatBoost
    - Justificativa da Escolha dos Modelos¶
  - Métricas de avaliação
    - Matriz de Confusão
    - Accuracy (Acurácia)
    - Precision (Precisão)
    - Recall (Revocação)
    - F1-SCORE
    - AUC (Area Under the Curve)
  - Treinamento dos modelos
    - Configuração dos Modelos
    - Validação Cruzada com *Oversampling*
    - Validação Cruzada com *Undersampling*
    - Comparação de Desempenho Entre as Técnicas
- **9. Otimização de Hiperparâmetros**
  - Configuração dos Hiperparâmetros
  - Aplicação de Técnica para Otimização
- **10. Avaliação dos Modelos XGBoost e Random Forest Otimizados**
  - Aplicação dos Modelos aos Dados de Teste
  - Desempenho dos Modelos com Métricas Iniciais
  - Importância dos Atributos
  - Desempenho dos Modelos com Matriz de Confusão
  - Desempenho dos Modelos com ROC e AUC
- **11. Conclusão**
