# Actividad 1.3.1 LAMP

Vamos a realizar la instalación de la pila LAMP en nuestro servidor de AWS. para ello instalaremos Apache2 y php.

Primero actualizamos los repositorios con el siguiente comando.
``` 
apt update
```
Una vez hecho esto instalamos Apache2 y php.

![Imagen](img/c1.PNG "Imagen")
![Imagen](img/c2.PNG "Imagen")

Ahora vamos a editar el sitio web por defecto. Este sitio se encuentra en ```/etc/apache2/sites-available``` y modificamos el fichero 000-default.conf para que quede de la siguiente manera.

![Imagen](img/c3.PNG "Imagen")

Lo siguiente es reiniciar el servicio apache2 con el siguiente comando:
``` 
systemctl restart apache2
```

Ahora vamos a hacer la comprobación de LAMP stack. Para ello vamos a crear una página de prueba para testear php en el "documentroot" del sitio web por defecto. El archivo debe tener lo siguiente:

![Imagen](img/c4.PNG "Imagen")

Comprobamos que se ha realizado correctamente al abrir la página web que muestra lo siguiente:

![Imagen](img/c5.PNG "Imagen")

Ahora procederemos con la instalacion del MARIADB. Para ello tenem