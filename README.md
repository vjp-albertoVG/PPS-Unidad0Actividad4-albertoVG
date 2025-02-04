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


