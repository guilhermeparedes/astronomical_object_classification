# [Classificação de Objetos Astronômicos](https://github.com/guilhermeparedes/astronomical_object_classification)


<div style="text-align: center;">
<img src="[https://imgs.search.brave.com/-hqie94eaXZazDLbGljPZx5InDwUruJRguqtwVtZyQQ/rs:fit:860:0:0:0/g:ce/aHR0cHM6Ly9oZWxp/b3MtaS5tYXNoYWJs/ZS5jb20vaW1hZ2Vy/eS9hcnRpY2xlcy8w/NUZTQk9RcjVKRXVU/SncwNUhkbGpMNi9p/bWFnZXMtMS5maWxs/LnNpemVfMjAwMHgy/MDAwLnYxNzE2MzE0/NDc3LmpwZw](https://github.com/user-attachments/assets/819c33dd-c80b-4011-ac00-ba4398ed0d4c)" alt="star" width="400"/>
</div>

## Objetivo

O **objetivo** deste projeto é a classificação de objetos celestes em estrelas, galáxias ou quasares utilizando diferentes modelos de
classificação supervisionados e métricas de avaliação. 

## Modelos
 
### Random Forest

### XGBoost

### LGBM 

### CatBoost 

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
