# Prueba T茅cnica Backend Node.js

Hola! 馃憢 Nos alegra que hayas llegado hasta este punto y puedas llegar a ser parte del gran equipo humano de Serempre.



## Entregables

- Repositorio GIT con c贸digo fuente
- Scripts SQL para la creaci贸n de la Base datos, creaci贸n de las tablas e insertado de datos



## Extras

En caso de que quieras correr la milla extra puedes realizar estos puntos extra:

- Documentaci贸n del API Swagger, ReDoc o Postman
- Implementar contenedores con Docker
- Desplegar en un servidor web Azure App Service, AWS, Google Cloud, Heroku o Netlify etc.
- Pruebas Unitarias
- Uso de TypeScript
- Utilizar una soluci贸n con ORM (Object-relational mapping)
- Uso de alg煤n framework de tu conocimiento (Nest, Sails, Adonis)



## Desarrollo de la prueba

### Base de datos

1. Crear la siguiente estructura de base datos en SQL a partir de siguiente diagrama:

<img src="./assets/erd.png" alt="Diagrama Modelo Entidad Relaci贸n" style="zoom:150%;" />

2. usar SQL Server (Recomendada), MySQL, PostgreSQL para la base de datos.
3. Importa los datos de las tablas usando los CVS en la carpeta [assets/data](./assets/data) (opcional).



### Servicio web

Realizar un Web API en Node.js express, debe tener los siguientes recursos disponibles :

>   *Para los campos que contengan ??? debes implementar una soluci贸n*

| Resource    | Endpoint                    | Request                                                      | Response                                                     | Descripci贸n                                                  |
| :---------- | --------------------------- | :----------------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Productos   | api/products?               | [Query](https://es.wikipedia.org/wiki/Query_string) : pagina, tama帽o de pagina, descendente | [Ver ejemplo](./assets/responses/products/products-1.json)   | Obtiene el listado de productos con su categor铆a ordenados de forma (as)(des)cendete por id             |
| Productos   | api/products/search?        | Query : nombre producto, nombre categor铆a, nombre proveedor  | [Ver ejemplo](./assets/responses/products/products-2.json)   | Permite realizar una b煤squeda por nombre de producto o categor铆a o proveedor (requiere amenos un filtro) |
| Productos   | api/products/:id            | URL : ID del producto                                        | [Ver ejemplo](./assets/responses/products/products-3.json)   | Obtiene la informaci贸n un producto con su categor铆a y proveedor |
| Productos   | api/products                | Body : datos de producto, id categor铆a y id proveedor<br />[Ver ejemplo](./assets/responses/products/products-4.json) | ???                                                          | Permite crear un nuevo producto con su categor铆a y proveedor |
| Productos   | api/products/:id            | URL : ID del producto<br />Body : datos de producto a actualizar<br />[Ver ejemplo](./assets/responses/products/products-5.json) | ???                                                          | Permite actualizar los datos de un producto                  |
| Categor铆as  | api/categories/:id/products | URL : ID categor铆a<br />Query : pagina, tama帽o de pagina     | [Ver ejemplo](./assets/responses/categories/categories-1.json) | Obtiene la informaci贸n de una categor铆a, con sus productos asociados |
| Proveedores | api/suppliers/:id           | URL : ID proveedor                                           | [Ver ejemplo](./assets/responses/suppliers/suppliers-1.json) | Obtiene la informaci贸n de un proveedor                       |
| Proveedores | api/suppliers/:id/products  | URL : ID proveedor                                           | [Ver ejemplo](./assets/responses/suppliers/suppliers-2.json) | Obtiene la informaci贸n de un proveedor con sus productos     |
| Proveedores | api/suppliers/:id           | URL : ID proveedor                                           | ???                                                          | Permite eliminar un proveedor                                |

>   *toma los ejemplos como referencias*

## A tener en cuenta

- C贸digo Limpio
- Excelentes pr谩cticas
- Implementar arquitectura escalable
- Uso de c贸digos de estado respuesta HTTP
- Uso de m茅todos para peticiones HTTP
- Validaci贸n de datos
- Manejo de errores
- El uso de patrones de dise帽o como ejemplo: SOLID, KISS DRY, MVC etc.
- Documentaci贸n de c贸digo



## Recomendaciones

- IDE para administrar bases de datos [DataGrip](https://www.jetbrains.com/datagrip/)
- Versiones de BD : MySQL 8, MSSQL 2017-2019, PostgreSQL 13



## Para enviar tu soluci贸n

Incluye un README.md que incluya la documentaci贸n acerca del proyecto, que hable de las cosas interesantes con las que te enfrentaste, decisiones que tomaste, etc. Cuando termines, crea un repositorio publico en GitHub que solo contenga tu proyecto.
