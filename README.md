# Ejecicios basicos con Gitlab

## Pasos ha realizar en git lab
- Primero pasamos a realizar la creacion del repositorio desde la pagina web una vez hemos entrado pulsando en create poject ![GitHub Logo](/images/logo.png)
- Tenemos que pulsar en **Create blanck project** insertar imagen
- Ahora se nos habre automáticamente una ventana en la cual tenemos que darle un nombre al proyecto que en este caso será **ejerciciosbasico**, dejamos la opción de private por defecto y pulsamos en create project insertar imagen
- Una vez hemos pulsado en create project nos saldra la siguiente imagen verificando oque se ha creado el proyecto correctamente insertar imagen

## Pasos a realizar en la máquina local antes de subir los archivos a git lab
- Creamos una carpeta nueva llamada subidagitlab con el comando **mkdir** "se tiene que crear como sudo" insertar imagen
- Ahora desde el propio terminar entramos a la carpeta con el comando **cd** y el nombre de la carpeta a la cual queremos entrar "si la capeta no está en la ubicacion donde nosotros estamos en la consola tendremos que escribir la ruta entera para poder situarnos dentro de ella" insertar imagen
- Una vez dentro crearemos con el comando sudo **touch / nano /vi** algun docuemto para asi poder hacer la prueba de la subida de archivos y usamos el comando **ls** para verificar que se han creado correctamente insertar imagen

## Pasos a realizar para la subida a gitlab
- Primero tenemos que añadir el proyecto al control de versiones de git con el comando **sudo git init** para esto tenemos que estar dentro de la carpeta que queremos añadir, que en este caso es subidagitlab
- Una vez añadido el proyecto al control de versiones hacemos el comando**git status** y vemos que el archivo que hemos creado antes no esta añadido al proyecto
- Para añadir el archivo al proyecto tenemos que usar el comando **git add "nombre del archivo"**
- Volvemos a hacer un **git status** y vemos que se ha sincronizado correctamente
- Ahora pasamos a registrar cambios en el historial con el comando **git commit -m "Comentario asociado"** y vemos que se ha realizado correctamente
- Una vez hemos hecho el comit tenemos que hacer que esta carpeta apunte remotamente al repositorio de git lab con el comando **git remote origin https://gitlab.com/atorresrod1/ejerciciosbasico.git **
- Ahora toca subir el archivo a gitlab a traves del comando **git push origin master**

## Comprobarque se ha subido el archivo a gitlab
- A simple vista parece que no se ha subido, pero es debido a que estamos viendo la rama del **main** y nosotros lo hemos subido a la rama de **master** para ver si realmente se ha subido selecionaremos la rama master
- una vez que se ha cargado la rama podemos ver que se ha subido correctamente
