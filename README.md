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

3.1. Utilização de 30% do dataset para a construção do modelo

3.2. Remoção de missing values e caracteres especiais

3.3. Remoção de caracteres de quebra de linha

3.4. Todas as reviews foram padronizadas (traduzidas) na língua inglesa

3.5. Tokenização

3.6. Remoção de stop words

3.7. Lemetização

3.8. Stemming
  
## 5. Conclusão

Neste estudo, a classificação de OCT foi realizada com modelos de aprendizado profundo e algumas abordagens foram testadas até que se chegasse ao modelo de melhor performance. Na primeira etapa, os dados foram padronizados e, em seguida, usados como entrada para a CNN Xception pré-treinada com os pesos do dataset ImageNet. 

Para validação, foi utilizada a técnica de validação cruzada estratificada com 5 folds e a divisão aleatória do dataset em subsets de treino, validação e teste. As duas abordagens apresentaram resultados similares.

O desempenho do modelo foi medido utilizando as métricas: acurácia, precisão e recall. Sendo recall a mais importante para o nosso conjunto de dados, pois devemos considerar o diagnóstico errado prejudicial, principalmente a classificação de uma imagem com uma das três anomalias como uma imagem normal. Apresentou bons resultados para a classificação de imagens das classes NORMAL e CNV e o pior resultado para as imagens da classe DRUSEN. 

