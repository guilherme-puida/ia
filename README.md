# Wine Revisor Predictor

## Integrantes

| Alunos                            |
| --------------------------------- |
| André Corrêa                      |
| Felipe Candido                    |
| Gabriel Mariano                   |
| Guilherme Puida                   |
| Lucas Gabriel                     |
| Mariana Rio                       |

## Sobre

Este projeto tem por objetivo o desenvolvimento de um modelo baseado em aprendizado de máquina para a efetiva qualificação de vinhos com base em uma série de atributos dos mesmos. A partir da seleção de três base de dados, foram aplicadas técnicas de tratamento de dados e em seguida utilizadas no treinamento de uma série de modelos de machine learning para a escolha do mais adequado para o problema supracitado. Com o intuito de se obter um modelo capaz de predizer, com um erro mínimo possível, a qualidade dos vinhos considerados.

## O projeto foi divido nas seguintes etapas:

### Aquisição de dados:

 - Wine Reviews [(Kaggle)](https://www.kaggle.com/datasets/zynicide/wine-reviews?select=winemag-data-130k-v2.csv)
 - Wine Quality [(UC Irvine)](https://archive.ics.uci.edu/dataset/186/wine+quality) e [(Kaggle)](https://www.kaggle.com/datasets/rajyellow46/wine-quality)
 - Wine Reviews Data [(Kaggle)](https://www.kaggle.com/datasets/samuelmcguire/wine-reviews-data)

### Exploração e preparação dos dados:

 - [Wine Reviews](https://github.com/guilherme-puida/ia/blob/main/notebooks/preparacao/wine_reviews.ipynb)
 - [Wine Quality](https://github.com/guilherme-puida/ia/blob/main/notebooks/preparacao/Preparacao_WineQuality.ipynb)
 - [Wine Reviews Data](https://github.com/guilherme-puida/ia/blob/main/notebooks/preparacao/Wine_Reviews_Data.ipynb)

### Seleção inicial dos modelos

 - [Wine Reviews](https://github.com/guilherme-puida/ia/blob/main/notebooks/selecao_modelos/Selecao_Modelos_Minemag_Data.ipynb)
 - [Wine Quality](https://github.com/guilherme-puida/ia/blob/main/notebooks/selecao_modelos/Selecao_Modelos_Wine_Quality.ipynb)
 - [Wine Reviews Data](https://github.com/guilherme-puida/ia/blob/main/notebooks/selecao_modelos/Selecao_Modelos_Wine_Review_Data.ipynb)

### Otimização e ajuste fino do sistema

 - [Wine Reviews](https://github.com/guilherme-puida/ia/blob/main/notebooks/otimizacao_modelos/Otimizacao_Winemag_Data.ipynb)
 - [Wine Quality](https://github.com/guilherme-puida/ia/blob/main/notebooks/otimizacao_modelos/Otimizacao_Modelos_WineQuality.ipynb)
 - [Wine Reviews Data](https://github.com/guilherme-puida/ia/blob/main/notebooks/otimizacao_modelos/Otimizacao_Modelos_Wine_Review_Data.ipynb)


##  Conclusões 

Por fim, foi escolhido o dataset Wine Quality, tendo em vista o baixo erro obtido com o mesmo a partir do treinamento de uma série de modelos de machine learning (em especial os modelos Random Forest Regressor e XGB Regressor) os quais obtiveram os menores erros para os testes realizados e a característica dos dados presentes na base de dados, os quais são mais voltados para um lado físico-químico da composição dos vinhos. 

A partir do mesmo, foi possível obter um Erro Quadrático Médio de aproximadamente 0.35, utilizando-se de uma escala que varia de 0 a 10 para atribuição de notas aos vinhos.

Deste modo, a partir do trabalho desenvolvido, conseguimos obter o resultado esperado, obtendo como resultado um modelo capaz de predizer com um erro mínimo a nota dada a um vinho com base em seus atributos físico-químicos.
