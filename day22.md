# git fetch and git merge (GIT PULL)
Estos comandos son la fusion del que llamamos ahora `git pull`.

## git fetch
Permite traer los cambios sin fusionarlo`(merge)` a nuestro repositorio local.

## git merge
Permite fusionar los cambios que tenemos de nuestro repositorio local que pedimos con un git fetch , puedes indicar la rama a unir.
Normalmente se usa la rama origin/master o origin/main.


```js
//Solicitar los cambios con un fetch
$ git fetch

//Fusionar los cambios con un merge
$ git merge origin/master


//Para resumir estos dos pasos colocariamos 
$ git pull
```
## #Dia22LearningGit