# API REST Y APRENDIZAJE AUTOMÁTICO
## Entorno Virtual - Local
La API va a realizar predicciones sobre la especie de una flor: largo y ancho del sépalo, y largo y ancho del pétalo. 

Se preentrenarán cuatro modelos distintos de clasificación, y se almacenarán en archivos .h5 para ser utilizados posteriormente por la aplicación.


La API tendrá 4 endpoints, uno por modelo:

`/predict/logistic`

`/predict/randomforest`

`/predict/svm`

`/predict/tree`

Se reciben los 4 parámetros (`sepal_length`, `sepal_width`, `petal_length`, `petal_width`) por query parameters o JSON.

## Archivos
- Descargar la carpeta llamada *models*
- Visualizar un archivo llamado *requirements.txt* que contenga lo siguiente:
_flask_
_scikit-learn_
_joblib_
- Visualizar un archivo llamado *iris_models.py*que contenga el código ya generado.

## Instalación
Crear un entorno virtual de Anaconda (Python) 

Moverse a la carpeta _machine__learning_api_ creada donde se encuentra la carpeta _models_

Instalar los módulos necesarios ejecutando `pip install -r requirements.txt`

## Modelos de Machine Learning
Generar los modelos de machine learning ejecutando en el cmd dentro de la carpeta _machine__learning_api_  `python iris_models.py` 
## Levantar el servidor
Para levantar el servidor ejecutamos: `python app.py`
Una vez que te aparezca la ruta puedes visualizarla (debe ser algo asi:  http://127.0.0.1:5001/ y tendrá que decir) "API DE PREDICCIÓN DE LA FLOR IRIS"

## Docker
Visualizar los archivos Docker y docker-compose.yml de la carpeta _machine__learning_api_ donde también se encuentra _models_
Docker-compose es una herramienta que te permite definir y ejecutar aplicaciones multicontenedor con Docker usando un único archivo de configuración. 
`docker-compose.yml`, es ideal para aplicaciones que necesitan varios servicios, como una API con Flask y una base de datos (como PostgreSQL o MongoDB).

## Levantar en Docker 
- Abrir Docker-Desktop
- Ejecutar: `docker-compose up --build` en terminal (consola o cmd) y en la carpeta _machine__learning_api_


### CRÉDITOS
(https://miguelevangelista.gitbook.io/herramientasavanzadas/ejemplos/api-rest-and-machine-learning/deploy-in-render)
