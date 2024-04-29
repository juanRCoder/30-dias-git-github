# gitignore, alias y git reflog:
Tu puedes decidir que archivos subir al servidor de github para eso existe un archivo que puede ignorar archivos o carpetas en especificos.

## gitignore:
El gitignore es un archivo especial de git que ignora ciertos archivos que tu coloques dentro de el, se escribe colocandole un punto antes asi: `.gitignore`.<br/>
Por ejemplo.
```js
//,gitignore
*.txt   // -> elimina todos los archivos del repositorio que terminen con .txt.
folder/ // -> elimina la carpeta en especifico y todos sus sub-archivos.
!archivo20.txt  // -> colocando un ! antes del archivo le decimos que no ignore este archivo en especifico.
```

## alias en git:
Podemos configurar alias a ciertos comandos muy largos por ejemplo al mostrar el historial de todos los cambios en las diferentes ramas.
```js
//Comando para ver todos los cambios en las diferentes ramas
$ git log --oneline --all --graph
"
*  (HEAD -> main) 6eb52 merge branch rama-b
|\
| * 57511 (rama-b) actualizacion actual
* | 432db commit rama b
* | d13c9 optimizando funcion saludar
|/
* 193da creando funcion saludar
"

//Configurar un alias para ese comando.
$ git config --global alias.log-simple "log --oneline --all --graph"

//Ahora solamente colocamos:
$ git log-simple
"
*  (HEAD -> main) 6eb52 merge branch rama-b
|\
| * 57511 (rama-b) actualizacion actual
* | 432db commit rama b
* | d13c9 optimizando funcion saludar
|/
* 193da creando funcion saludar
* 695fa agregando folder repo/
* 2s2da agregando funcion sumar
"
```

## git reflog
git reflog nos permite ver todas las posiciones en que se movio el puntero HEAD, en este caso miremos un ejemplo practico. comando `git reflog`.

Eliminamos un cambio(commit)
```
$ git reset --hard commit
```
Pero por error lo elimine quiero volver y quiero restablecerlo.
```js
//Hacemos un git log-simple y no se mostrar el commit porque lo eliminamos.
$ git log-simple
6eb52 (HEAD -> main) cambio actual

//Entonces hacemos un git reflog para ver todas las posiciones del HEAD.
$ git reflog 
"
6eb52 (HEAD -> main) HEAD@{0}: cambio actual
4cbe4 HEAD@{1}: commit eliminado
"

//En ese historial podremos ver el hash del commit eliminado y solamente lo resetamos.
$ git reset --hard 4cbe4
HEAD is now at 4cbe4 commit eliminado

```
## #Dia8LearningGit
# gitignore, alias y git reflog:
Tu puedes decidir que archivos subir al servidor de github para eso existe un archivo que puede ignorar archivos o carpetas en especificos.

## gitignore:
El gitignore es un archivo especial de git que ignora ciertos archivos que tu coloques dentro de el, se escribe colocandole un punto antes asi: `.gitignore`.<br/>
Por ejemplo.
```js
//,gitignore
*.txt   // -> elimina todos los archivos del repositorio que terminen con .txt.
folder/ // -> elimina la carpeta en especifico y todos sus sub-archivos.
!archivo20.txt  // -> colocando un ! antes del archivo le decimos que no ignore este archivo en especifico.
```

## alias en git:
Podemos configurar alias a ciertos comandos muy largos por ejemplo al mostrar el historial de todos los cambios en las diferentes ramas.
```js
//Comando para ver todos los cambios en las diferentes ramas
$ git log --oneline --all --graph
"
*  (HEAD -> main) 6eb52 merge branch rama-b
|\
| * 57511 (rama-b) actualizacion actual
* | 432db commit rama b
* | d13c9 optimizando funcion saludar
|/
* 193da creando funcion saludar
"

//Configurar un alias para ese comando.
$ git config --global alias.log-simple "log --oneline --all --graph"

//Ahora solamente colocamos:
$ git log-simple
"
*  (HEAD -> main) 6eb52 merge branch rama-b
|\
| * 57511 (rama-b) actualizacion actual
* | 432db commit rama b
* | d13c9 optimizando funcion saludar
|/
* 193da creando funcion saludar
* 695fa agregando folder repo/
* 2s2da agregando funcion sumar
"
```

## git reflog
git reflog nos permite ver todas las posiciones en que se movio el puntero HEAD, en este caso miremos un ejemplo practico. comando `git reflog`.

Eliminamos un cambio(commit)
```
$ git reset --hard commit
```
Pero por error lo elimine quiero volver y quiero restablecerlo.
```js
//Hacemos un git log-simple y no se mostrar el commit porque lo eliminamos.
$ git log-simple
6eb52 (HEAD -> main) cambio actual

//Entonces hacemos un git reflog para ver todas las posiciones del HEAD.
$ git reflog 
"
6eb52 (HEAD -> main) HEAD@{0}: cambio actual
4cbe4 HEAD@{1}: commit eliminado
"

//En ese historial podremos ver el hash del commit eliminado y solamente lo resetamos.
$ git reset --hard 4cbe4
HEAD is now at 4cbe4 commit eliminado


//Ahora si tendremos
4cbe4 (HEAD -> main) commit eliminado
6eb52 cambio actual
```
## #Dia8LearningGit