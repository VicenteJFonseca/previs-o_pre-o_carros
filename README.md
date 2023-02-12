# Machine Learning para previsão de preços FIPE

## Descrição

Modelo de Machine Learning para a previsão da média de preços do índice FIPE (Fundação Instituto de Pesquisas Econômicas) que, por sua vez, considera as seguintes variáveis:<br>

1 - Ano de referência (year_of_reference); <br>
2 - Mês de referência (moth_of_reference); <br>
3 - Código FIPE para o modelo do carro (fipe_code);<br>
4 - Autentificação da FIPE para consulta no site (authentication);<br>
5 - Marca (brand);<br>
6 - Modelo do carro (model);<br>
7 - Tipo de combustível (fuel);<br>
8 - Tipo de direção (gear);<br>
10 - Tamanho do motor (gear);<br>
11 - Ano do modelo (year_model);<br>
12 - Mês de referência (moth_of_reference);<br>
13 - Média de preço mensurada pela FIPE (avg_price_brl).

## Resumo

Foi utilizado o Google Colab para a prototização do modelo bem como também o Drive como repositório para a base de dados. Por conseguinte, pode-se enumerar as seguintes etapas para o modelo de machine learning desenvolvido. <br>

1 - Visualização dos dados: utilização de algumas bibliotecas python para visualização de dados como o seaborn para analizar as variáveis numéricas; checagem dos tipos de características; aplicação do Pandas Profile para uma apreensão ágil e abrangente de todas as *features* do problema de negócio em questão.<br>
2 - Pré-processamento dos dados: tratamento de variáveis categóricas com categorias subrepresentadas; seleção de variáveis com a exclusão de *features* que possuem as seguintes implicações: alta correlação que pudessem incorrer  multicolinearidade; inócuas para determinação da target como a coluna de códigos de identificação; binarização das variáveis categóricas que permaneceram no modelo; transformação Yeo-Johnson nas variáveis numéricas para tornar os dados mais próximos de uma distribuição normal; Padronização de todas as variáveis para evitar escalas discrepantes entre os dados.<br>
3 - Versionamento: utilização da ferramenta DagsHub e do MLflow para versionamento do modelo.<br> 
4 - Treinamento e escolha dos modelos: Foi definido os conjuntos de treino e teste. Foram treinados modelos regressores e a avaliação do desempenho dos mesmos foi por meio do RMSE



