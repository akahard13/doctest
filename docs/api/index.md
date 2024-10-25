---
sidebar_position: 1
---
# Introducción


Este proyecto se hizo con la intención de mejorar tanto la lógica como el rendimiento del **Sistema de becas** de la **UNAN - León**, utilizando **PHP 8.3.11** que hasta la fecha de hoy **24 de Octubre de 2024** es la versión **latest**, esta versión de php de la mano con el **Framework Laravel** en su versión **11.9** apoyados de su documentación.

Para mantener este sistema en orden y con la intención de encontrar las tablas con facilidad se creó un nuevo esquema dentro de la base de datos **prematric** llamado **sistema_becas**, ahí podemos encontrar absolutamente todas las tablas a excepción de la tabla **matricula** esta se encuentra en el esquema **public** y no se pudo sacar porque cambiaria mucho el funcionamiento de otros sistemas que tambié usan esta base de datos.

El orden que se maneja entre archivos es: **Controllers -> Services -> Models**, todo esto desde la carpeta app. Ahora bien, el controlador se encarga de llamar a las funciones que se encargan del procesado de los datos en cuestión ya sea mediante el **ORM Eloquent** también de laravel o haciendo uso de los modelos directamente según convenga.