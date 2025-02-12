# Classificação de Objetos Astronômicos

## Modelos: 

- Definição - Modelo : Random Forest 

- Definição - Modelo : XGBoost

- Definição - Modelo : SVC (Support Vector Machine Classifier)

- Definição - Modelo : Naive Bayes

- Definição - Modelo : KNN (k-nearest neighbors)

- Definição - Modelo : LGBM (light...)


O **objetivo** deste trabalho é realizar a previsão , baseada nas observações anteriores, utilizando como métrica accuracy, f1, precision, recall e roc_auc.

## Dependências
- ```pandas```: para leitura e manipulação dos dados
- ```numpy```: para realizar operações em array
- ```matplotlib```: para visualizações estáticas ou interativas
- ```seaborn```: para criar gráficos de forma eficiente e visualmente atraente
- ```sklearn```: para criar, treinar e implementar modelos de aprendizado de máquina

## Estrutura do projeto
# 1. Introdução
As características espectrais são fundamentais para diferenciar distintos tipos de objetos celestes, como estrelas, galáxias e quasares. As estrelas emitem radiação eletromagnética de maneira semelhante a um corpo negro, exibindo linhas de absorção específicas. No caso das galáxias, o seu espectro é resultado da soma dos espectros de todas as estrelas e de demais materiais radiantes que as compõem. Os quasares, por outro lado, apresentam linhas de emissão marcantes, frequentemente acompanhadas por um desvio expressivo para o vermelho (redshift).

# 2. Contexto do dataset

Este exercício tem como objetivo classificar um conjunto de 100 mil objetos celestes em três categorias: estrelas, galáxias e quasares. Os dados utilizados foram extraídos da [versão 17 do Sloan Digital Sky Survey (SDSS)](https://www.sdss3.org/dr17/), um projeto internacional que reúne imagens captadas por telescópios localizados na América do Norte e na América do Sul. Cada objeto no catálogo é descrito por 17 atributos (features), além de uma coluna que identifica sua respectiva categoria.

##    2.1 Por que estes estudos são importantes?

Categorizar objeto astronômicos com base em suas características espectrais é crucial para o entendimento da evolução estelar e formação de galáxias.

# 3. Dados

- **obj_ID:** Identificador do objeto, um valor único que identifica o objeto no catálogo de imagens utilizado pelo arquivo de dados do Sloan Digital Sky Survey (SDSS).

- **alpha:** Ângulo de Ascensão Reta (em graus) na época J2000, um sistema de coordenadas amplamente utilizado em astronomia para descrever a posição de objetos celestes no céu.

- **delta:** Ângulo de Declinação (em graus) na época J2000, outro sistema de coordenadas comumente usado em astronomia para localizar objetos celestes.

- **u, g, r, i, z:** Filtros fotométricos usados no sistema SDSS para medir a quantidade de luz emitida pelos objetos em diferentes faixas de comprimento de onda. Cada filtro corresponde a uma cor específica da luz: u no ultravioleta, g no verde, r no vermelho, i no infravermelho próximo e z no infravermelho.

- **run_ID:** Número de execução que identifica uma varredura específica do céu realizada pelo SDSS. Cada varredura cobre uma região determinada do céu e recebe um número único.

- **rereun_ID:** Número de reprocessamento que indica como a imagem foi processada, incluindo a versão do software ou o método de calibração utilizado na criação da imagem.

- **cam_col:** Coluna da câmera, usada para identificar a linha de varredura dentro da execução. Cada varredura é dividida em múltiplas colunas da câmera para cobrir uma área maior do céu.

- **field_ID:** Número do campo, utilizado para identificar cada campo dentro da varredura. O campo representa uma região menor dentro da coluna da câmera.

- **spec_obj_ID:** Identificador único para objetos espectroscópicos ópticos. Isso significa que duas observações diferentes com o mesmo spec_obj_ID devem pertencer à mesma classe de objeto, que pode ser galáxia, estrela ou quasar.

- **class:** Classe do objeto, a classificação atribuída ao objeto com base em suas propriedades espectrais. Pode ser uma galáxia, uma estrela ou um quasar.

- **redshift:** Valor do desvio para o vermelho, baseado no aumento do comprimento de onda da luz emitida pelo objeto devido ao seu movimento em relação ao observador. Esse valor mede a expansão do universo desde o momento em que a luz foi emitida pelo objeto.

- **plate:** Identificador da placa utilizada na pesquisa espectroscópica do SDSS. Cada placa contém múltiplas fibras que coletam a luz de diferentes objetos.

- **MJD:** Data Juliana Modificada, utilizada para indicar quando um determinado conjunto de dados do SDSS foi coletado. É uma versão modificada da Data Juliana, um sistema padronizado para representar datas e horários em astronomia.

- **fiber_ID:** Identificador da fibra óptica que direcionou a luz para o plano focal durante cada observação. Cada fibra coleta a luz de um objeto diferente, permitindo que o SDSS observe vários objetos simultaneamente.

Mais informações sobre as características espectrais de objetos celestes podem ser encontradas [aqui](https://www.sdss3.org/dr9/imaging/imaging_basics.php)

# 4. Objetivo do estudo
O objetivo deste projeto é a classificação de objetos celestes em estrelas, galáxias ou quasares utilizando diferentes modelos de
classificação supervisionados e métricas de avaliação. 

5. Importação de bibliotecas
6. Leitura dos dados
7. Análise descritiva geral
8. Proposta de um Modelo Baseline
9. Proposta de um modelo mais complexo
10. Conclusão
11. Sugestão de outros modelos
