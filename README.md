# Práctica 13 - Creación de una base de datos con Azure COSMOS DB

En la barra de búsqueda de [Azure](https://portal.azure.com/) buscamos el _Azure Cormos DB_.

![Práctica 13 - Parte 1](imagenes\p13p1.png)

Vamos a crear una base de datos con núcleo SQL.

![Práctica 13 - Parte 2](imagenes\p13p2.png)

Configuramos los parámetros:
- Suscripción
- Grupo de recursos: sesion6
- Nombre de la cuenta: cosmosdb321
- Ubicación
Aplicamos el descuento de nivel gratis y dejamos los demás parámetros iguales.

![Práctica 13 - Parte 3](imagenes\p13p3.png)

Debemos verificar que en redes estén activas Todas las redes.

![Práctica 13 - Parte 4](imagenes\p13p4.png)

Una vez creado el recurso, nos metemos a él, elegimos una plataforma Node.js y creamos el contenedor "Items", luego seleccionamos el navegador web.

![Práctica 13 - Parte 5](imagenes\p13p5.png)

Nos dará la bienvenida y podremos selecconar los items.

![Práctica 13 - Parte 6](imagenes\p13p6.png)

Dentro de los items seleccionamos "New Item".

![Práctica 13 - Parte 7](imagenes\p13p7.png)

Creamos un nuevo item con el código:
{
    "id": "1",
    "nombre": "karen",
    "apellido": "vera"
}
y lo guradamos.

![Práctica 13 - Parte 8](imagenes\p13p8.png)

El item se guardará con líneas agregadas por el Node.js

![Práctica 13 - Parte 9](imagenes\p13p9.png)

Podemos crear otro item con los mismos parámetros, incluso podemos agregar otro como:
"perrito": "Happy"

![Práctica 13 - Parte 10](imagenes\p13p10.png)

Para poder ver estos items podemos seleccionar "New SQL Query".

![Práctica 13 - Parte 11](imagenes\p13p11.png)

Con _SELECT * FROM c_ podemos ver todos los items que se han creado.

![Práctica 13 - Parte 12](imagenes\p13p12.png)

Para ver un solo item podemos poner el código:
SELECT * FROM c where c.id="1"

![Práctica 13 - Parte 13](imagenes\p13p13.png)