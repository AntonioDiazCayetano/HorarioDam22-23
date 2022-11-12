# Ejercicio A y B, formas para realizarlo:

Primero se debe abrir un directorio donde introduciremos nuestros archivos con los que vamos a trabajar.
Por consiguiente haremos click con el botón derecho y señalaremos >Git Bush Here.

![image](https://user-images.githubusercontent.com/114742418/201344784-c2839340-a967-455c-bfb8-75ee6161c1c7.png)


## GIT INIT

![image](https://user-images.githubusercontent.com/114742418/201343859-a7728cfe-51b6-4988-a4e7-bfc86d06eed3.png)

Al comienzo de todo proyecto se introduce este comando para Git haga un seguimiento del proyecto.  Aquí se ha creado el repositorio internamente aunque nosotros no veamos nada en el editor o en nuestro directorio. Si optamos por ver los archivos ocultos de nuestra carpeta ahí sí encontraremos nuestra carpeta con toda la información de Git.

## GIT STATUS -S

![image](https://user-images.githubusercontent.com/114742418/201468833-7a68cd09-2c64-4373-b280-aafdbd784d68.png)

Nos muestras los archivos y carpetas que tenemos en nuestro directorio. Nos muestra una interrogación roja porque no están siendo sometidos a seguimiento por parte de Git.

## GIT COMMIT - M

![image](https://user-images.githubusercontent.com/114742418/201469112-1870c26a-1dc9-488d-8171-9f56b8487be6.png)

Traslada los archivos del área de ensayo al repositorio local. En este último lugar es donde se crea el respaldo. Además tenemos la posibilidad de ponerle un nombre al proyecto. Con este comando se consigue guardar cambios que hayamos realizado. En este caso podemos ver que un sólo archivo ha sido respaldado, el resto no. Si volvemos a realizar un Git Status -S veremos que ahora sólo nos informa que dos archivos no tiene seguimiento, los que tienen seguimiento desaparecen de esta lista.

## GIT LOG --ONELINE

![image](https://user-images.githubusercontent.com/114742418/201469548-bec10202-cbd7-4c64-a111-e6f1063fecb2.png)

Con este comando podemos ver una lista de los diferentes cambios realizados y en la rama que han sido efectuados, en este caso ha sido en la rama "master".

----------
#### Si deseamos subir los archivos a un repositorio de GitHub o GitLab debemos crear éste primeramente asignándole un nombre, lo creamos y después copiaremos la url que nos ha asignado para luego pegarla en la consola de Git.

![image](https://user-images.githubusercontent.com/114742418/201470621-4bda99f8-183b-4d42-9012-557c90f730da.png)

Si lo que buscamos es retroceder después de un cambio realizado pero teniendo en cuenta que no hemos hecho un add deberemos aplicar el comando:
#### <Git checkout más el nombre del archivo>. ####
Pero si en el caso de que hayamos realizado un add previamente y nos veamos obligados a retrocer en la línea de modificaciones se puede hacer un reset, para ello Git nos ofrece el comando: #### <git reset head más el nombre del archivo>. ####

Otro caso que se puede dar es querer volver a una modificación en concreto, las cuales están numeradas con un identificador. Este identificador nos ayudará a la hora de aplicar el comando de tal manera: #### < git checkout y el identificador >. ####





