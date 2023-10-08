# Registro y Login usando Laravel PHP

Esta aplicación web permite a un usuario entrar en la web principal y, desde ahí, registrarse o iniciar sesión con sus credenciales.

## Tecnologías empleadas

La aplicación está realizada con

-   PHP
-   Laravel y sus dependencias

Para más información, consultar el archivo "Readme-laravel.md".

## Base de Datos e instalación de dependencias

Para probar el funcionamento en un entorno local es necesario:

-   Clonar o desargar este repositorio.
-   Crear una base de datos con MySQL (o similar) con el comando "CREATE DATABASE {nombre_database};"
-   Crear en la raíz del proyecto un archivo ".env" tomando como base el archivo .env.example.
-   Actualizar el archivo .env recién creado con el nombre de la base de datos creada y los datos de acceso a la misma (usuario y contraseña).

-   Abrir una terminal en la raíz del proyecto clonado/descargado.
-   Instalar las dependencias ejecutando los siguientes comandos en una terminal.
    -   composer install #dependencias de Composer (PHP)
    -   npm install #dependencias de Node.js
    -   php artisan key:generate #generar una clave de aplicación ("APP_KEY" en el archivo .env)
    -   php artisan migrate #Ejecutar las migraciones de la base de datos
    -   php artisan serve #levantar el servidor. Devuelve la ruta de acceso (debería ser "http://127.0.0.1:8000").
-   Abrir otra terminal en la raíz del proyecto y ejecutar el comando:
    -   npm run dev #compilar los recursos de front-end

## Ejecución

-   Abrir un navegador e ir a la dirección que ha devuelto el comando "php artisan serve" (debería ser "http://127.0.0.1:8000").
-   Las rutas http://127.0.0.1:8000/login y http://127.0.0.1:8000/register deberían dirigir a las páginas de login y registro, respectivamente. También se pueden acceder a las rutas indicadas a través de los enlaces "Log in" y "Register", en la página principal.

Con estos pasos debería ser posible registrar usuarios y autenticarlos en el sistema.

Cada vez que se desee poner en funcionamento la apliación, una vez hecho los pasos anteriores, será suficiente ejecutar los comandos "php artisan serve" y "npm run dev" en terminales diferentes abiertas dentro la raíz del proyecto.
