# Primer Proyecto Parcial: Modelado de Temas

**Autores:** <br/>
Isabel Navarro  A00823132. <br/>
Oscar Peña A01176808. <br/>
Ernesto Guzmán A00824855. <br/>
Natalia González A01382007 <br>
Alexa Mercado A01634000 <br>

## Data Scrapping

En el documento scrapping.ipynb se utiliza la libreria de Tweepy y PRAW para buscar los posts y tweets de un usuario en especifico. Además, se les hace un 
procesamiento para anonimizar cualquier información sensible e hipervínculos. En el caso de Reddit, también se  remueven  menciones  a  otros  subreddits  y  menciones  a  otros usuarios. 

### Innovación 1

Además de buscar tweets y posts también busca comentarios de Youtube.


## BERTopic

BERTopic es una técnica de modelado de temas que aprovecha las incrustaciones de BERT y un TF-IDF basado en clases para crear grupos densos que permiten temas fácilmente interpretables mientras se mantienen las palabras importantes en las descripciones de los temas. A cada uno de los conjuntos de datos de las redes sociales (Twitter, Reddit y Youtube) se la aplica  un modelado  de  temas dinámico y un modelado de temas estático de su contenido.

## Hierarchical Dirichlet Process

El proceso jerárquico de Dirichlet (HDP) es un poderoso modelo de membresía mixta para el análisis no supervisado de datos agrupados. A diferencia de su contraparte finita, la asignación latente de Dirichlet, el modelo de tema HDP infiere la cantidad de temas a partir de los datos, no se le asigna. A cada uno de los conjuntos de datos de las redes sociales (Twitter, Reddit y Youtube) se la aplica el modelado de temas de HDP.

## Innovación 2: Latent Semantic Analysis

## Innovación 3: Non-Negative Matrix Factorization

El método de non-negative matrix factorization es un método de modelado de temas que cae debajo de clustering de la libreria de scikit-learn. Transforma un grupo de diferentes documentos en unos que se pueden resumir como una mezcla de temas que son una mezcla de palabras. Como la mayoría de los algoritmos de aprendizaje automático, NMF funciona comenzando con una suposición de valores para W y H, y minimizando iterativamente la función de pérdida. Por lo general, se implementa actualizando una matriz (ya sea W o H) para cada iteración y continúa minimizando la función de error, ||V — WH || = 0, mientras que los valores de W y H permanecen no negativos, hasta que W y H sean estables.

## Resultados de los modelos utilizados

Para probar los modelos se utilizo la cuenta de Twitter de Joe Biden para los 3 modelos.

BERTopic:

HDP: Como conclusiones, el modelo de HDP no es ideal para este tipo de conjunto de datos ya que, como se observa en la visualización de resultados del documento HDP_model.ipynb, las palabras en cada topic no se agruparon de la manera más óptima.

NMF: Como conclusiones, el modelo funciona muy bien en separar las palabras en temas como se observa en la visualización de resultados del documento NMF_Model.ipynb. Las palabras se agrupan de manera muy óptima.
