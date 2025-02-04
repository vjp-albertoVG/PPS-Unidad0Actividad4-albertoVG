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

![](imagenes/imagen1gloval.png)

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
![](imagenes/crearrepositorio4.png)
