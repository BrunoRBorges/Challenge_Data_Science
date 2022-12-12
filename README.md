# Challenge_Data_Science
#Problema

A imobiliária InsightPlaces, situada na cidade do Rio de Janeiro, está enfrentando dificuldades para alugar e vender imóveis. Em uma pesquisa de como empresas semelhantes operam no mercado, a InsightPlaces percebeu que esse problema pode estar relacionado aos valores dos imóveis e às recomendações que faz.

Dentro desse contexto, como podemos definir de forma eficiente os preços dos imóveis lidando com grande volume de dados? É importante recomendar imóveis utilizando outro critério? O que precisa ser feito?

Faço parte do time de Ciência de Dados e Big Data da InsightPlaces e fiquei responsável por auxiliar no processo de análise de dados dos imóveis localizados em alguns bairros da cidade do Rio de Janeiro.

Esse projeto tem algumas etapas como: ler e fazer o tratamento do histórico dos preços de imóveis no Rio de Janeiro, construir um modelo de regressão para precificar imóveis e criar um recomendador de imóveis. Para cada uma dessas etapas vou utilizar a ferramenta PySpark que oferece uma melhor performance ao trabalharmos com grandes volumes de dados.

#Semana 01 

Na semana 01, tratei os dados recebidos em arquivos .json utilizando o PySpark, retirei do banco de dados alguns tipos de imóveis, como comerciais e lançamentos, devido a sua baixa significância no grupo total de dados, e depois gerei um arquivo .parquet para continuar os trabalhos na semana 02.

#Semana 02

Na semana 02, retomei o trabalho do ponto de parada da semana 01, terminei de tratar as informações de dados e colunas, colocando todas nos tipos corretos e criando colunas dummy baseadas em alguns tipos de dado. Depois, utilizei a biblioteca de machine learning do PySpark para tentar criar um adivinhador de preço de imóveis, utilizei o PCA e o Standard Scaler para reduzir a quantidade de hiperparâmetros, e comparei as análises do Linear Regressions com a GBTRegressor.

#Semana 03

Na semana 03, peguei o arquivo da semana 02 com as colunas dummy, reduzi a quantidade de hiperparâmetros com Standard Scaler e PCA, e utilizei o Kmeans para criar clusters de imóveis "parecidos". Depois, criei um recomendador de imóveis baseado em seu ID, criei um pipeline para essas transformações e analisei o resultado dos clusters.
