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
**Si deseamos subir los archivos a un repositorio de GitHub o GitLab debemos crear éste primeramente asignándole un nombre, lo creamos y después copiaremos la url que nos ha asignado para luego pegarla en la consola de Git.**

![image](https://user-images.githubusercontent.com/114742418/201470621-4bda99f8-183b-4d42-9012-557c90f730da.png)

Si lo que buscamos es retroceder después de un cambio realizado pero teniendo en cuenta que no hemos hecho un add deberemos aplicar el comando:
**Git checkout más el nombre del archivo.**
Pero si en el caso de que hayamos realizado un add previamente y nos veamos obligados a retrocer en la línea de modificaciones se puede hacer un reset, para ello Git nos ofrece el comando: **git reset head más el nombre del archivo.**

Otro caso que se puede dar es querer volver a una modificación en concreto, las cuales están numeradas con un identificador. Este identificador nos ayudará a la hora de aplicar el comando de tal manera: **git checkout y el identificador.**

## Git Clone

![image](https://user-images.githubusercontent.com/114742418/201473946-f4de84ad-fabd-40e0-a42b-2a09ec3fc78c.png)

Con este comando podremos hacer una copia en nuestro directorio si hemos sufrido, por ejemplo, un borrado de todo el material. Cuando ingresamos **git clone más la url** recibiremos una copia exacta de los archivos eliminados dentro del directorio donde sufrimos el desastre.

#Parte B del ejercicio:

En esta parte me ha vuelto a dar los mismos errores que en la parte A. Cuando voy a subir algo al Git no me lo permite y debo realizarlo a mano pero en cambio me dice que el directorio está creado. He visto que tengo realizado un push en Github y eso no me permite subir nada a Gitlab ya que me da error, pero tampoco sé eliminar ese push:
Aquí adjunto la consola con la información para mostrar que está creado el directorio y demás.

![image](https://user-images.githubusercontent.com/114742418/201476826-07600d0d-0dd4-4404-b857-d122670a9bfe.png)


![image](https://user-images.githubusercontent.com/114742418/201474956-60f2079e-7c28-4b07-8673-a0db79b4488a.png)

**Me informa que hay un segundo push en mi rama principal de Github, o así lo entiendo, y además que la rama no está protegida**


# REVISAR COMMITS REALIZADOS

Realizaremos un **git log --oneline** para comprobar los commit que tenemos realizados con sus respectivas modificaciones e identificadores asignados a éstas:

![image](https://user-images.githubusercontent.com/114742418/201475390-99b6edcf-83a9-42b5-b35b-87f6ad7b2cf2.png)

Después de realizar un **git checkout más el identificador de la modificación** me encuentro en una línea de tiempo anterior:

![image](https://user-images.githubusercontent.com/114742418/201475489-0a7b5917-aece-45b4-8abf-d018c78acb2b.png)

Como podemos ver en la siguiente captura, me encuentro en el identificador elegido:

![image](https://user-images.githubusercontent.com/114742418/201475523-1dd69a9b-865c-461d-b239-166b2fad06cb.png)

Hemos vuelto al principio de la rama master y para ello hemos usado el comando **git checkout master**

![image](https://user-images.githubusercontent.com/114742418/201475578-99e48bf9-54bb-41fc-8da7-d27c7147d80d.png)

En el último paso podemos ver que todo continúa en su lugar y nada ha sido modificado, para divisar esto se aplica el comando **git log --oneline**:

![image](https://user-images.githubusercontent.com/114742418/201475635-5eed2ba7-2240-43df-b82a-26c47bfef44e.png)




