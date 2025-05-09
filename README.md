# TpGestionPeliculas

Trabajo practico para gestionar peliculas en una bsae de datos consultando y agregando las mismas

# Requisitos

Java (JDK 17 o superior)

IntelliJ IDEA

MySQL (servidor local o remoto)

Postman

Maven

# Instrucciones 

Descargar zip
Descomprimir
Abrir en IDE
Correr proyecto

#Endpoints

Crear una nueva película  
POST http://localhost:8080/peliculas

Body (JSON):  
{
  "titulo": "Interstellar",
  "director": "Christopher Nolan",
  "anio": 2014,
  "genero": "Ciencia Ficción"
}

Respuesta esperada:  
{
  "id": 1,
  "titulo": "Interstellar",
  "director": "Christopher Nolan",
  "anio": 2014,
  "genero": "Ciencia Ficción"
}

--------------------------------------------------

Obtener todas las películas  
GET http://localhost:8080/peliculas

Respuesta esperada:  
[
  {
    "id": 1,
    "titulo": "Interstellar",
    "director": "Christopher Nolan",
    "anio": 2014,
    "genero": "Ciencia Ficción"
  }
]

--------------------------------------------------

Obtener una película por su ID  
GET http://localhost:8080/peliculas/1

Respuesta esperada:  
{
  "id": 1,
  "titulo": "Interstellar",
  "director": "Christopher Nolan",
  "anio": 2014,
  "genero": "Ciencia Ficción"
}

--------------------------------------------------

Obtener películas por año  
GET http://localhost:8080/peliculas/anio/2014

Respuesta esperada:  
[
  {
    "id": 1,
    "titulo": "Interstellar",
    "director": "Christopher Nolan",
    "anio": 2014,
    "genero": "Ciencia Ficción"
  }
]
