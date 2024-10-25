---
sidebar_position: 4
---
# Models

Se encuentran en la carpeta **app/Models** del proyecto, divididos en 2 secciones, una carpeta llamada **/sb_periodo** donde se encuentran todos los modelos relacionados con la confirmación de los periodos de solicitud de becas y los modelos relacionados a toda la parte administrativa del sistema, también está una carpeta llamada **/sb_solicitud** donde se encuentra todo lo relacionado a la gestión, guardado y todo el procesamiento de las solicitudes de becas que realizan los estudiantes.

## Tipos de modelos

### Modelos de consulta

Estos modelos son los que solamente vamos a utlizar para acceder a su información, pero no no vamos ni a insertar ni a actualizar sus datos por medio de la api, en este tipo de modelos solo se define el nombre de la tabla con su esquema para poder acceder a ella, por ejemplo:

![img](/img/modelo_consulta.png)

### Modelos de consulta relacionados

Estos modelos sirven como consulta y como modificadores de las tablas, pueden insertar y actualizar según se usen, pero para mantener un orden y relación de datos entre tablas se les define sus relaciones a otras tablas, en este tipo de modelo aparte de las relaciones se definen los campos que van a ser rellenables, la llave primaria, si hará uso de timestamps (es decir si la tabla tiene los campos **created_at** y **updated_at**) y al igual que en el tipo de modelo anterior se define el nombre de la tabla con su esquema, por ejemplo:

![img](/img/modelo_consulta_relacionado.png)
