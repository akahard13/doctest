---
sidebar_position: 2
---
# API Docs

Este proyecto se hizo con la intención de mejorar tanto la lógica como el rendimiento del **Sistema de becas** de la **UNAN - León**, utilizando **PHP 8.3.11** que hasta la fecha de hoy **24 de Octubre de 2024** es la versión **latest**, esta versión de php de la mano con el **Framework Laravel** en su versión **11.9** apoyados de su documentación.

Para mantener este sistema en orden y con la intención de encontrar las tablas con facilidad se creó un nuevo esquema dentro de la base de datos **prematric** llamado **sistema_becas**, ahí podemos encontrar absolutamente todas las tablas a excepción de la tabla **matricula** esta se encuentra en el esquema **public** y no se pudo sacar porque cambiaria mucho el funcionamiento de otros sistemas que tambié usan esta base de datos.

El orden que se maneja entre archivos es: **Controllers -> Services -> Models**, todo esto desde la carpeta app. Ahora bien, el controlador se encarga de llamar a las funciones que se encargan del procesado de los datos en cuestión ya sea mediante el **ORM Eloquent** también de laravel o haciendo uso de los modelos directamente según convenga.

## Modelos

Se encuentran en la carpeta **app/Models** del proyecto, divididos en 2 secciones, una carpeta llamada **/sb_periodo** donde se encuentran todos los modelos relacionados con la confiruación de los periodos de solicitud de becas y los modelos relacionados a toda la parte administrativa del sistema, también está una carpeta llamada **/sb_solicitud** donde se encuentra todo lo relacionado a la gestión, guardado y todo el procesamiento de las solicitudes de becas que realizan los estudiantes.

### Tenemos 2 tipos de modelos:

#### Modelos de consulta:

Estos modelos son los que solamente vamos a utlizar para acceder a su información, pero no no vamos ni a insertar ni a actualizar sus datos por medio de la api, en este tipo de modelos solo se define el nombre de la tabla con su esquema para poder acceder a ella, por ejemplo:

![img](/img/modelo_consulta.png)

#### Modelos de consulta relacionados:

Estos modelos sirven como consulta y como modificadores de las tablas, pueden insertar y actualizar según se usen, pero para mantener un orden y relación de datos entre tablas se les define sus relaciones a otras tablas, en este tipo de modelo aparte de las relaciones se definen los campos que van a ser rellenables, la llave primaria, si hará uso de timestamps (es decir si la tabla tiene los campos **created_at** y **updated_at**) y al igual que en el tipo de modelo anterior se define el nombre de la tabla con su esquema, por ejemplo:

![img](/img/modelo_consulta_relacionado.png)
