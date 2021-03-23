# Prueba Técnica Backend Node.js

Hola! 👋 Nos alegra que hayas llegado hasta este punto y puedas llegar a ser parte del gran equipo humano de Serempre.

## Entregables

- Repositorio GIT con código fuente
- Scripts sql para la creacion de la Base datos, creacion de las tablas e insertado de datos

## Extras

- Documentación del API Swagger, ReDoc o Postman
- Implementar contenedores con Docker
- Desplegar en un servidor web Azure App Service, AWS, Google Cloud, Heroku o Netlify etc.
- Pruebas Unitarias
- Uso de TypeScript
- Implementar una solucion con ORM (Object-relational mapping)
- Uso de algun framework de tu conocimiento (Nest, Sails, Adonis)

## Desarrollo de la prueba

### Base de datos

- Crea tu base de datos en SQL a partir del siguiente diagrama :

![Diagrama Modelo Entidad Relación](./assets/erd.png)

- puedes usar SQL Server (Recomendada), MySQL, Postgresql o Oracle DB para tu base de datos.

- Importa los datos de las tablas con los CVS (opcional).

### Servicio web

Crea una aplication web API en Node.js que tenga los siguientes recursos disponibles :

| Recurso   	| Endpoint            	| Peticion                                          	| Descripcion 	| Respuesta 	|
|-----------	|---------------------	|---------------------------------------------------	|-------------	|-----------	|
| Productos 	| api/products        	| QueryParams : (pagina, cantidad items por pagina) 	|             	|           	|
| Productos 	| api/products/:id    	| Params : (id de producto)                         	|             	|           	|
| Productos 	| api/products/search 	| QueryParams                                       	|             	|           	|
|           	|                     	|                                                   	|             	|           	|
|           	|                     	|                                                   	|             	|           	|

## A tener en cuenta

- Codigo Limpio
- Excelentes prácticas
- Implementacion de arquitectura escalable
- Uso de codigos de estado respuesta HTTP
- Uso de metodos para peticiones HTTP
- Validacion de datos
- Manejo de errores
- El uso de patrones de diseno SOLID, KISS DRY, MVC etc.
- Documentacion de codigo

## Recomendaciones

- IDE para administrar bases de datos [DataGrip](https://www.jetbrains.com/datagrip/)

## Para enviar tu solución

Incluye un README.md que incluya la documentacion acerca del proyecto, que hable de las cosas interesantes con las que te enfrentaste, decisiones que tomaste, etc. Cuando termines, crea un repositorio publico en GitHub que solo contenga tu proyecto.
