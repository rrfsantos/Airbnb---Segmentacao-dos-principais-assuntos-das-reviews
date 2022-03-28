## Airbnb - Segmentação dos principais assuntos das reviews utilizando Latent Dirichlet Allocation (LDA)



### 1. Itens do trabalho:

* Análise exploratória dos dados

* Tratamento dos dados para uso na modelo LDA

* Utilização de GridSearchCV para encontrar melhor modelo LDA

* Avaliação do modelo utilizando Probabilidade logarítmica e Perplexidade


### 2. Descrição dos dados

O dataset é composto por reviews do site Airbnb, para apartamentos localizados no Rio de Janeiro.

> Inside Airbnb: http://insideairbnb.com/get-the-data.html

## 3. Modelagem

Neste estudo, a foi utilizada a técnica não supervisionada de modelagem de tópicos Latent Dirichlet Allocation (LDA), para a segmentação dos principais assuntos das reviews.

[Notebook 1 - Limpeza e pré processamento do texto das reviews](https://github.com/rrfsantos/Airbnb-Segmentacao-dos-principais-assuntos-das-reviews/blob/main/1_Airbnb_pre_processamento.ipynb)

* Utilização de 30% do dataset para a construção do modelo

* Remoção de missing values e caracteres especiais

* Remoção de caracteres de quebra de linha

* Todas as reviews foram padronizadas (traduzidas) na língua inglesa

* Tokenização

* Remoção de stop words

* Lemetização

* Stemming

[Notebook 2 - Latent Dirichlet Allocation (LDA) e WordCloud](https://github.com/rrfsantos/Airbnb-Segmentacao-dos-principais-assuntos-das-reviews/blob/main/1_Airbnb_pre_processamento.ipynb)

* Vetorização das palavras das reviews

* Utilização de GridSearchCV para encontrar melhor modelo LDA

* Utilização do o modelo LDA com maior probabilidade logarítmica e menor perplexidade

* Visualização dos tópicos (assuntos) via pyLDAvis

* WordCloud
  
### 4. Conclusão



