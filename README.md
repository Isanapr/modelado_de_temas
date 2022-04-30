# Primer Proyecto Parical: Modelado de Temas

**Autores:** <br/>
Isabel Navarro  A00823132. <br/>
Oscar Peña A01176808. <br/>
Ernesto Guzmán A00824855. <br/>
Natalia González A01382007 <br>

## Data Scrapping

En el documento scrapping.ipynb se utiliza la libreria de Tweepy y PRAW para buscar los posts y tweets de un usuario en especifico. Además, se les hace un 
procesamiento para anonimizar cualquier información sensible e hipervínculos. En el caso de Reddit, también se  remover  menciones  a  otros  subreddits  y  menciones  a  otros usuarios. 

### Inovación 1

Además de buscar tweets y posts también busca comentarios de Youtube.


## BERTopic

BERTopic es una técnica de modelado de temas que aprovecha las incrustaciones de BERT y un TF-IDF basado en clases para crear grupos densos que permiten temas fácilmente interpretables mientras se mantienen las palabras importantes en las descripciones de los temas. A cada uno de los conjuntos de datos de las redes sociales (Twitter, Reddit y Youtube) se la aplica  un modelado  de  temas dinámico y un modelado de temas estático de su contenido.

## Hierarchical Dirichlet Process

El proceso jerárquico de Dirichlet (HDP) es un poderoso modelo de membresía mixta para el análisis no supervisado de datos agrupados. A diferencia de su contraparte finita, la asignación latente de Dirichlet, el modelo de tema HDP infiere la cantidad de temas a partir de los datos, no se le asigna. A cada uno de los conjuntos de datos de las redes sociales (Twitter, Reddit y Youtube) se la aplica el modelado de temas de HDP.

Como conclusiones, el modelo de HDP no es ideal para este tipo de conjunto de datos ya que, como se observa en la visualización de resultados del documento HDP.ipynb, las palabras en cada topic no se agruparon de la manera más óptima.


