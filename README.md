# SRI-Apache-PHP
El objetivo es levantar un contenedor de docker con un servidor apache+php y mostrar un Hola Mundo.

Para levantar el servicio crearemos un documento "docker-compose.yml" el cual configuraremos con los siguientes parametros:
-Versión: 3.9

-Servicios

  -Nombre de la imagen: php:7.4-apache
  
  -Nombre del contenedor: asir_apache+php
  
  -Puertos: 80:80
  
  -Volumenes:
  
    ./html:/var/www/html
    
    ./confapachephp:/etc/apache2

Para comprobar si esta correcto tendremos que iniciar el contenedor y luego ir al navegador y buscar "localhost:80" y se nos mostrara el Hola mundo.
