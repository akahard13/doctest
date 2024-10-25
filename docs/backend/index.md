---
sidebar_position: 1
---
# Introduccion


Este proyecto se hizo con la intención de mejorar tanto la lógica como el rendimiento del **Sistema de becas** de la **UNAN - León**, utilizando **PHP 8.3.11** que hasta la fecha de hoy **24 de Octubre de 2024** es la versión **latest**, esta versión de PHP de la mano con el **Framework Laravel** en su versión **11.9** apoyados de su documentación.

Para mantener este sistema en orden y con la intención de encontrar las tablas con facilidad se creó un nuevo esquema dentro de la base de datos **prematric** llamado **sistema_becas**, ahí podemos encontrar absolutamente todas las tablas a excepción de la tabla **matricula** esta se encuentra en el esquema **public** y no se pudo sacar porque cambiaría mucho el funcionamiento de otros sistemas que también usan esta base de datos. El orden que se maneja entre archivos es: **Controllers -> Services -> Models**, todo esto desde la carpeta app.

**NOTA:**
Cabe destacar que la clave **jwt** que se usa para encriptar y desencriptar los tokens de inicio de sesión para mayor seguridad se encuentra ubicado en la carpeta **/config**:

![img](/img/jwt.png)