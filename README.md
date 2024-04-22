# EVALUACIÓN SEMANA 5 - TESTING MOVIE API

El entregable consiste en crear los tests para la API de movie realizada en el 3.

Debe haber como mínimo estos 19 tests:

# Actors
GET /actors
POST /actors
DELETE  /actors/:id
PUT /actors/:id

# Genres
GET /genres
POST /genres
DELETE  /genres/:id
PUT /genres/:id

# Directors
GET /directors
POST /directors
DELETE  /directors/:id
PUT /directors/:id

# Movies
GET /movies
POST /movies
DELETE  /movies/:id
PUT /movies/:id
POST /movies/:id/actors
POST /movies/:id/directors
POST /movies/:id/genres

# CRITERIOS DE EVALUACIÓN:

Hay 19 test, cada uno vale 0.53 pts




# Template de Servidor Express y Sequelize

Este es un template básico para un servidor Express con sequelize con configuraciones comunes. Utiliza las siguientes librerías:

* cors (v2.8.5): Middleware para permitir solicitudes HTTP desde diferentes dominios.

* dotenv (v16.3.2): Carga variables de entorno desde un archivo .env.

* express (v4.18.2): Marco web minimalista para la construcción de aplicaciones web y API.

* helmet (v7.1.0): Middleware que ayuda a proteger las aplicaciones Express configurando varios encabezados HTTP.

* pg (v8.11.3): Controlador de PostgreSQL para Node.js.

* pg-hstore (v2.3.4): Serializador/deserializador para datos JSON y hstore en PostgreSQL.

* sequelize (v6.35.2): ORM para interactuar con bases de datos relacionales.


## Instalación

1. Clona este repositorio:

```bash
git clone https://github.com/Generacion-32/exp-sq-g32.git <NOMBRE_DEL_PROYECTO>
cd <NOMBRE_DEL_PROYECTO>

```
2. Tambien puedes hacerlo con el siguiente comando

```
npx exp-sq-g32
```

## Uso

>Para usar este template debes contar o crear una base de datos.

### Modo de Desarrollo

Para ejecutar el servidor en modo de desarrollo, utiliza:

```
npm run dev
```
Esto iniciará el servidor con Nodemon, que reiniciará automáticamente la aplicación cuando detecte cambios en el código.

## Modo de Producción

Para ejecutar el servidor en modo de producción, utiliza:

```
npm start
```

Este comando ejecutará la aplicación en un entorno de producción.

## Contribuciones

¡Las contribuciones son bienvenidas! Si encuentras algún problema o tienes sugerencias para mejorar el template, no dudes en comunicarla.

## Licencia
Este proyecto está bajo la Licencia ISC 



Crear una API para una aplicación de películas

Genres
name 

Actors
firstName
lastName
nationality
image
birthday

Directors
firstName
lastName
nationality
image
birthday

Movies
name
image
synopsis
releaseYear

Crear las relaciones: una película puede tener muchos actores, muchos directores y ser de muchos géneros. 

Cada modelo debe tener sus endpoints para un CRUD.

Para el endpoint GET -> /movies, cada película debe traer sus géneros, actores y directores.

Adicionalmente, añadir los siguientes endpoints

POST -> /movies/:id/genres para modificar los géneros de una película.

Debe recibir body de números, que serán los id’s de los géneros a los que pertenece esa película.

A su vez, debe retornar los géneros recién añadidos en un arreglo. 
 



Los siguientes endpoints también deben cumplir con las instrucciones mencionadas anteriormente. 

POST -> /movies/:id/actors para modificar los actores de una película

POST -> /movies/:id/directors para modificar los directores de una película

Conectar la API con este frontend y corroborar que todo esté funcionando correctamente: https://github.com/Generacion-34/week3-entregable-frontend.git 



