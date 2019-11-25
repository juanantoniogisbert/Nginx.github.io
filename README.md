## SITIO 1

NGINX, es un famoso software de servidor web de código abierto. En su versión inicial, funcionaba en servidores web HTTP. Sin embargo, hoy en día también sirve como proxy inverso, balanceador de carga HTTP y proxy de correo electrónico para IMAP, POP3 y SMTP. Fue lanzado oficialmente en octubre del 2004. El creador del software, Igor Sysoev, comenzó su proyecto en el 2002 como un intento de solucionar el problema C10k.

Para instalar nginx solamente tendremos que hacer el siguiente comando

```markdown
$ sudo apt-get install nginx
```

Como hemos echo en la parctica de [apachae](https://juanantoniogisbert.github.io/Apache.github.io/) crearemos un fichero index.php en la carpeta `/var/www/sitiophp`

### Estar publicada en el puerto 82

En el fichero default de nginx cambiaremos el puerto.

![Alt text](images/cap1.png?raw=true "Title")

### El directorio donde se encuentra el contenido del sitio será /var/www/sitioPhp

Ahora indicaremos nuestro directorio

![Alt text](images/cap2.png?raw=true "Title")


### Los logs se sitúan en el directorio /etc/logs/sitioPhp

Aqui en el fichero `nginx.conf` le indicaremos la ruta de nuestros logs.

![Alt text](images/cap3.png?raw=true "Title")


### Debe tener activada la compresión de ficheros que superen los 80kb

Seguiremos editando el mismo fichero y activamos la compresion y la capacidad.

![Alt text](images/cap4.png?raw=true "Title")

### Dispone de una página que se mostrará al acceder a una ruta que no exista.
Esta página (404.html) estará situada en /var/www/errores

Primeramente crearemos en /var/www el directorio errores, dentro pondremos nuestra pagina de error

![Alt text](images/cap5.png?raw=true "Title")


### No permita el acceso al contenido de nuestro servidor siempre que en el path
del contenido a obtener se encuentre la palabra private

![Alt text](images/cap6.png?raw=true "Title")
![Alt text](images/cap7.png?raw=true "Title")


## SITIO 2

### Estar publicada en el puerto 82

Hacemos el mismo proceso que en el sitio 1 pero poniendo el puerto 82.

![Alt text](images/cap8.png?raw=true "Title")

### El directorio donde se encuentra el contenido del sitio será /var/www/sitioNode

![Alt text](images/cap9.png?raw=true "Title")

### Los logs se sitúan en el directorio /etc/logs/sitioNode

![Alt text](images/cap10.png?raw=true "Title")


### Dispone de una página que se mostrará al acceder a una ruta que no exista.
Esta página (404.html) estará situada en /var/www/errores

![Alt text](images/cap11.png?raw=true "Title")
![Alt text](images/cap11.png?raw=true "Title")
