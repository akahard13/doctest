---
sidebar_position: 2
---

# Controllers

Ubicados en la carpeta **/app/Http/Controllers**,  dentro de esta tenemos 2 carpetas, la carpeta donde van a estar todos los controladores que hacen referencia a la configuración y manejo del sistema llamada **/administracion** y otra donde van a estar todos los controladores que se encargan de la gestión del procesado y manejo de las solicitudes del estudiante llamada **/solicitudes**, también contamos con controladores que se encunetran fuera de esas carpetas pero aún dentro de **/app/Http/Controllers**, estos controladores son de uso compartido, que contienen funciones que ocupan tanto la parte administrativa como la parte de solicitudes.

En los controladores solo encontraremos las funciones a las que mandamos a llamar en las rutas, aparte de su respectivo constructor generado con su o sus respectivos servicios a utilizar, por ejemplo:
