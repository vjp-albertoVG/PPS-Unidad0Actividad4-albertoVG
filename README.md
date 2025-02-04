# PPS-Unidad0Actividad4-albertoVG

Vamos a hacer una nueva actividad con git. En esta ocasión crearemos un pequeño proyecto de una página web que podremos visualizar creando un pequeño servidor con php.
Como en la actividad anterior el producto a realizar será el repositorio en github. Allí tendrás que documentar la realización de la práctica con la explicación del procedimiento, sus imágenes, etc.

## Seguimos configurando Git

Ya habrás configurado tu email y tu user con git config. Vamos a configurar algunas cosas más.

1. Configura el editor de comandos. Yo por simplicidad utilizaría nano ``git config — global core.editor nano``
1. Comprueba qué valor tienen las variables de configuración de git. Puedes utilizar la ayuda ``git config --help``.
1. Ajusta los valores de las  variables de Git:

~~~
color.status=auto
color.branch=auto
color.interactive=auto
color.diff=auto
~~~ 

![](imagenes/Imagenl.png)

## Creación de Proyecto y repositorio

Para ello crea una nueva carpeta en tu directorio de git de PPS, con el nombre de esta actividad ___PPSActividad4Unidad0RaulAlbalatPerez___

Creo un nuevo repositorio público con nombre **PPSActividad4Unidad0RaulAlbalatPerez-** 

Sigue las indicaciones de github para crear tu nuevo repositorio en linea de comandos, esto es:



Viene a ser como esto, pero cambiando el nombre de usuario y de repositorio:

~~~
echo "# PPSActividad4Unidad0RaulAlbalatPerez-> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:vjp-raulAP/PPSActividad4Unidad0RaulAlbalatPerez-.git
git push -u origin main
~~~

---
## Iniciando Proyecto 


1. Haz un listado en forma de arbol (tree -a) de todos los archivos del directorio.
	+ En la imagen aparece un listado de las carpetas creadas y las ramas creadas
  ![](imagenes/Imagen2.png)


2. Crea un archivo con nombre** README** (si no existe todavía) y lo añades al proyecto.
  ![](imagenes/Imagen3.png)
 

3. Comprueba el estado de git (`git status -s` o `git status --short``. 

  ![](imagenes/Imagen4.png)

4. Escribe en él una descripción de la actividad y vuelves a comprobar su estado.
![](imagenes/Imagen5.png)
![](imagenes/Imagen6.png)


## Ignorando archivos

1. Crea una carpeta con nombre** Excluded**. En ella vamos a colocar la documentación que no queremos que sea rastreada y subida al repositorio.
+ Creo la carpeta **Excluded** dentro del fichero del repositorio de la práctica
 
![](imagenes/Imagen7.png)

2. Para comprobar que funciona crea algún archivo vacío allí y también crea un archivo con nombre excluido.txt en el directorio principal del repositorio.

![](imagenes/Imagen8.png)

3. Crea un archivo con nombre **.gitignore** en el cual vamos a poner los archivos y directorios que no queremos que se rastreen.

![](imagenes/Imagen9.png)

4. Indica en el** .gitignore** que los archivos con extensión** .txt** y el directorio **Excluded** no deben de ser rastreados ni sincronizados..
+ En gitignore se encontrará los archivos de textos que no se verán 
![](imagenes/Imagen10.png)

5. Comprueba el estado del proyecto y comprueba que no nos indica nada del seguimiento de dichos archivos.
![](imagenes/Imagen11.png)


## Trabajo con Git

1. Crea un archivo con nombre index.html. 
Dentro de nuestro directorio de practica 4 nos creamos el archivo `touch index.html`.

![](imagenes/Imagen12.png)

3. Introduce el código html para que nos muestre un mensaje de Hola mundo con tu nombre. Uno sencillo sería este:
~~~
   <H1>Hola $USER¡¡¡ ¿Qué tal te encuentras?</H1>
~~~   
![](imagenes/Imagen13.png)

3. Visualiza el estado del proyecto ( puedes hacer tambien un git status corto ``git status --s` o `git status --short``). 
![](imagenes/Imagen14.png)

4. Puedes ver como te indica que tienes varias operaciones por hacer: git add, git commit...

5. Añade el archivo index.html al proyecto (git add).
6. Haz un commit (Puedes hacer ``commit -am "commentario del commit"` de esta manera se añaden las modificaciones de archivos y se hace el commit con el mensaje indicado sin abrir el archivo y tener que escribir nosotros).
![](imagenes/Imagen15.png)

7. Vuelve a comprobar el estado del proyecto. Puedes ver como ya debería de estar todo en orden.


8. Vuelve a subir los cambios a tu repositorio de github (git push)
![](imagenes/Imagen16.png)


## Creación de nuestro servidor web y visualización de nuestro proyecto


1. En un nueva pestaña de terminal y en el mismo directorio, ejecuta php -S 0:8080 para lanzar un servidor con la página html que has creado.

![](imagenes/Imagen17.png)
2. Visualiza la página creada Puedes acceder a ella en tu navegador en el puerto 8080 de tu equipo: [](http://localhost:8080)

![](imagenes/Imagen18.png)
![](imagenes/Imagen19.png)


## Seguimos Trabajando con Git

1. Haz una copia del archivo local** index.html** con el nombre** index.html.save.** Modifica el fichero index.html para que cambie el texto mostrado en la página web.

 ![](imagenes/Imagen20.png)

2. Verifica estado del proyecto.

 ![](imagenes/Imagen21.png)

+ Esto indica que index.html.save es un archivo nuevo no añadido al control de versiones.

3. Comprueba las diferencias de los archivos que no han sido añadidos (``git diff``)

![](imagenes/Imagen22.png)
+ Si index.html.save es idéntico a index.html, no verás diferencias. Si introduces cambios en index.html.save, este comando te mostrará los cambios.

4. Refresca navegador para comprobar que ha cambiado el contenido de nuestra página web.
 
![](imagenes/Imagen23.png)

5.  Vuelve a la versión anterior del archivo index.html (git restore).
 
![](imagenes/Imagen24.png)

6. Vuelve a refrescar navegador para ver como vuelve a versión inicial.

![](imagenes/Imagen25.png)

7. Vamos a utiliza el comando ``git mv``. Elimina el archivo index.html y después de hacer un commit, mueve el archivo con index.html.save a index.html
Eliminar index.html (aunque en realidad no es necesario eliminarlo antes de renombrarlo, Git lo maneja automáticamente cuando usamos git mv)


 ![](imagenes/Imagen26.png)

Renombra index.html.save a index.html con el comando git mv:

 ![](imagenes/Imagen27.png)

8. Mira el estado del proyecto y confirma todos los cambios.


9. Para pull y push, haz un push y comprueba cómo han subido los archivos a github.com.

![](imagenes/Imagen28.png)

10.  Modifica el archivo index.php desde la página de github.com y haz un pull y comprueba cómo se ha modificado la página web en nuestro navegador.

![](imagenes/Imagen29.png)

hacemos un pull con los cambios realizados en github y los guardamos.

![](imagenes/Imagen30.png)

comprobamos que se han modificado los cambios

![](imagenes/Imagen31.png)
 

