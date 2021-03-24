# Prueba Técnica Backend Node.js

Hola! 👋 Nos alegra que hayas llegado hasta este punto y puedas llegar a ser parte del gran equipo humano de Serempre.



## Entregables

- Repositorio GIT con código fuente
- Scripts SQL para la creación de la Base datos, creación de las tablas e insertado de datos



## Extras

En caso de que quieras correr la milla extra puedes realizar estos puntos extra:

- Documentación del API Swagger, ReDoc o Postman
- Implementar contenedores con Docker
- Desplegar en un servidor web Azure App Service, AWS, Google Cloud, Heroku o Netlify etc.
- Pruebas Unitarias
- Uso de TypeScript
- Utilizar una solución con ORM (Object-relational mapping)
- Uso de algún framework de tu conocimiento (Nest, Sails, Adonis)



## Desarrollo de la prueba

### Base de datos

1. Crear la siguiente estructura de base datos en SQL a partir de siguiente diagrama:

<img src="./assets/erd.png" alt="Diagrama Modelo Entidad Relación" style="zoom:150%;" />

2. usar SQL Server (Recomendada), MySQL, PostgreSQL o Oracle DB para la base de datos.
3. Importa los datos de las tablas usando los CVS en la carpeta [assets/data](./assets/data) (opcional).



### Servicio web

Realizar un Web API en Node.js express, debe tener los siguientes recursos disponibles :

>   *Para los campos que contengan ??? debes implementar una solución*

| Resource    | Endpoint                    | Request                                                      | Response                                                     | Descripción                                                  |
| :---------- | --------------------------- | :----------------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Productos   | api/products?               | [Query](https://es.wikipedia.org/wiki/Query_string) : pagina, tamaño de pagina, descendente | [Ver ejemplo](./assets\responses\products\products-1.json)   | Obtiene el listado de productos con su categoría             |
| Productos   | api/products/search?        | Query : nombre producto, nombre categoría, nombre proveedor  | [Ver ejemplo](./assets\responses\products\products-2.json)   | Permite realizar una búsqueda por nombre de producto o categoría o proveedor (requiere amenos un filtro) |
| Productos   | api/products/:id            | URL : ID del producto                                        | [Ver ejemplo](./assets\responses\products\products-3.json)   | Obtiene la información un producto con su categoría y proveedor |
| Productos   | api/products                | Body : datos de producto, id categoría y id proveedor<br />[Ver ejemplo](./assets\responses\products\products-4.json) | ???                                                          | Permite crear un nuevo producto con su categoría y proveedor |
| Productos   | api/products/:id            | URL : ID del producto<br />Body : datos de producto a actualizar<br />[Ver ejemplo](./assets\responses\products\products-5.json) | ???                                                          | Permite actualizar los datos de un producto                  |
| Categorías  | api/categories/:id/products | URL : ID categoría<br />Query : pagina, tamaño de pagina     | [Ver ejemplo](./assets\responses\categories/categories-1.json) | Obtiene la información de una categoría, con sus productos asociados |
| Proveedores | api/suppliers/:id           | URL : ID proveedor                                           | [Ver ejemplo](./assets\responses\suppliers\suppliers-1.json) | Obtiene la información de un proveedor                       |
| Proveedores | api/suppliers/:id/products  | URL : ID proveedor                                           | [Ver ejemplo](./assets\responses\suppliers\suppliers-2.json) | Obtiene la información de un proveedor con sus productos     |
| Proveedores | api/suppliers/:id           | URL : ID proveedor                                           | ???                                                          | Permite eliminar un proveedor                                |

>   *toma los ejemplos como referencias*

## A tener en cuenta

- Código Limpio
- Excelentes prácticas
- Implementar arquitectura escalable
- Uso de códigos de estado respuesta HTTP
- Uso de métodos para peticiones HTTP
- Validación de datos
- Manejo de errores
- El uso de patrones de diseño como ejemplo: SOLID, KISS DRY, MVC etc.
- Documentación de código



## Recomendaciones

- IDE para administrar bases de datos [DataGrip](https://www.jetbrains.com/datagrip/)



## Para enviar tu solución

Incluye un README.md que incluya la documentación acerca del proyecto, que hable de las cosas interesantes con las que te enfrentaste, decisiones que tomaste, etc. Cuando termines, crea un repositorio publico en GitHub que solo contenga tu proyecto.