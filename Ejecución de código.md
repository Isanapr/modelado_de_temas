# Ejecución del código:

## 1. scrapping.ipynb

- Reddit: Para correr esta sección se debe introducir el nombre del usuario de Reddit en “user” y al final se descargará un documento .csv con el nombre “user_Filtered_Reddit.csv”.
- Twitter: Para correr esta sección se debe introducir el nombre del usuario de Twitter en “user ID” y al final se descargará un documento .csv con el nombre “user_Filtered_TW.csv”.
- Youtube: Para correr esta sección se debe introducir el url del video de donde se desea extraer los comentarios y al final se descargará un documento .csv con el nombre “youtube_Filtered_YT.csv”.

Ya que se hayan descargado los tres documentos filtrados, se puede comenzar a aplicar el “topic modeling”. Los .csv deben estar en la misma ubicación de donde se correra el modelo.

## 2. BERTopic

## 3. HDP_Model

- En la sección de lectura de datos, se debe introducir el nombre del documento que se quiere analizar (“user_Filtered_Reddit.csv”, “user_Filtered_TW.csv” o “youtube_Filtered_YT.csv”) en la línea:

		df = pd.read_csv(‘name’,lineterminator='\n')

		reemplazando ‘name’ por el nombre del .csv.

## 4. LDA_model
* En la sección de lectura de datos, se debe introducir el nombre del documento que se quiere analizar (“user_Filtered_Reddit.csv”, “user_Filtered_TW.csv” o “youtube_Filtered_YT.csv”).
	La instruccion se encuentra en el segundo bloque del notebook LDA_model.ipynb
	
		`df= pd.read_csv('JoeBiden_Filtered_TW.csv')`
