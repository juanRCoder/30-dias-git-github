# ramas, fusion de ramas y sus derivados:
Una vez aprendido lo baico es hora de aprender un poco sobre las ramas , las diferentes versiones de un archivo que podemos trabajar en equipos de trabajo.

Estos son los comandos para las ramas y fusion de ramas en git.
```js
$ git branch            //Ver las ramas y la rama actual.
$ git branch ramab      //Crear una rama.
$ git switch ramab      //Cambiar de rama.
$ git switch -c ramac   //Crear y moverse a la rama.
$ git switch -d ramac   //Eliminar una rama.
$ git switch -D ramac   //Eliminar una rama de manera forzada (en caso extremo).
$ git branch -m ramab ramad //Cambiar de nombre a una rama.
$ git branch -m ramaf   //Cambiar de nombre de la actual rama.
$ git merge ramaf		//Agregar lo cambios de ramaf a rama principal.
$ git merge main 		//Extraer los archivos de la rama (b) a la rama principal (main).
```
OJO: Si cometiste algun error o te equivocaste al fusionar las ramas puedes aplicar un comando ya visto como:
```js
//hacemos un retroceso al commit anterior del merge para eliminar.
$ git reset --hard commit-anterior
```
## Flujo de trabajo (puede variar segun como trabajes).
Este es un flujo que podemos realizar para una trabajar con ramas.

```js
$ git switch -c ramaB	//rear e acceder a la nueva rama.

//Hacer los cambios, hacer un git add y luego un commit.

$ git switch main		//irse a la rama que quiere fusionar.
$ git pull			    //traer cambios si otro desarrollador ha hecho.
$ git merge ramaB		//traer los cambios a la rama principal.
```
Esto seria por el tema deramas, fusion de ramas y resolucion si hicimos un mal merge, cualquier cosita puedes consultar a la documentacion o enviarme un mensaje al discord: juanRCoder. :)
## #Dia6LearningGit