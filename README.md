README
# Descripción
Este es un proyecto CRUD implementado con Python, Flask y MongoDB. A continuación, se detallan los endpoints disponibles:
(Debe utilizar la URL que usted quiera utilizar)

## Crear Tarea
````
POST http://127.0.0.1:5000/todo/ 
Content-Type: application/json

{
    "title": "Example title",
    "description": "example description"
}
````

## Obtener Todas las Tareas
````
GET http://127.0.0.1:5000/todo/ 
````

## Obtener una Tarea Específica
````
GET http://127.0.0.1:5000/todo/:id
````

## Actualizar una Tarea
````
PUT http://127.0.0.1:5000/todo/:id
Content-Type: application/json

{
    "title": "Learn Python and Flask and something else",
    "done": "True"
}
````

## Eliminar una Tarea
````
DELETE http://127.0.0.1:5000/todo/:id
````

# Configuración del Entorno Virtual
Recomendamos crear un entorno virtual para este proyecto. Puede hacerlo ejecutando el siguiente comando:
````
python -m venv venv
````


## Para activar el entorno virtual, use el siguiente comando:
````
./venv/scripts/activate
````

## Instalación de Dependencias
Este proyecto tiene un archivo requirements.txt que contiene las dependencias necesarias. Puede instalarlas utilizando pip:

````
pip install -r requirements.txt
````

## Por Ultimo! .env

no olvidemos conectar nuestra base de datos, para este proyecto utilicé Mongodb atlas y agregé la URI para conectarse a la base de datos en un archivo .env en la raiz del repositorio
.env
MONGO_URI=mongodb+srv://<username>:<password>@cluster0.wk7ilvc.mongodb.net/pythonflaskdb

(custer0 default, modifiquelo si es necesario segun sus necesidades)
