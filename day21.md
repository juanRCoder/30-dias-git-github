# stage , commit and server
Estas son etapas que passa el archivo desde repositorio local a repositorio remoto.
Una vez hecho los cambios en nuestro repositorio local, quieres subir tu codigo a la plataforma de github, 
estas son las fases que pasa para ese proceso.

## zone stage:
Cuando haces un cambio lo primero que debes es agregar como lo siguiente:
```js
//Subir archivos a github
$ git add file.txt

//Despues de agregar verificas si el archivo esta en la zona
//Si es asi se marcara de verde

//Zona stage
+-----------------------------+
|  new File: file.txt         |
+-----------------------------+
```
## commit
Luego de desto envias el archivo con un mensaje especifico del porque y las caracteristicas del cambio hecho o realizado.
```js
//Declarar el tipo de cambio
$ git commit -m 'mensaje del cambio o archivo agregado'
```

## server
Despues de realizar comitear el archivo toca empujarlos al servidor de github o sea al repositorio remoto.
```js
//Empujar o enviar los archivos al servidor de github
$ git push
```
## #Dia21LearningGit