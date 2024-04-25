# Git pull - forks. 
Cuando estamos trabajando en grupos soleamos subir cambios el archivo que se nos hace tedioso ver los cambios de otros o avisar cuando hicimos cambios.

Para esto existe un comnado que nos actualiza el repositorio remoto para luego trabajar en lo mas actualizado.

Usamos para eso ``git pull``.
```js
//Comando nos actualizar el repositorio remoto
$ git pull 
```

### forks:
Que es un fork , es simplemente una copia de un repositorio existente osea una copia del proyecto de otra persona.

Podemos clonar el proyecto de otra persona nediante github.
Solamente buscamos un proyecto:
1. Buscamos la opcion ``Fork``.
2. Ya estaremos haciendo la copia, ahora solamente cambiamos el nombre o la descripcion del proyecto paa tenerlo nosotros.
3. Asi listo ya habremos fork(bifurcado) un proyecto ajeno.

## Flujo de trabajo (actualizado)
Llegado a este punto ya podemos actualizar el flujo de trabajo.
```js
//Antes que nada hacemos un git pull para ver actualizar
$ git pull
//Agregamos nuestro archivo
$ git add [file]
//Comiteamos nuestro archivo
$ git commit -m '[mensaje de commit]'
//verificamos
$ git status -s
//Hacemos otro git pull verificando actualizaciones en el archivo
$ git pull
//Finalmente subimos el archivo al repositorio remoto
$ git push
````
Espero este flujo ayude a todo el lo lea.

## #Dia10LearningGit