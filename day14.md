# Git stash && cherry-pick
Esta parte es necesaria para guardar datos temporalmente o 

# git stash
permite guardar cambios temporales mientras trabajamos en otro coas como en otra rama o en otros archivos, etc.
Luego cuando queremos aplicarlos regresamos donde hicimos el ``git stash`` y aplicamos este comando ``git stash pop``

```js
//Guardar lo scambios de un archivo no comiteado
$ git stash

//Hacer operaciones o trabajo en otras ramas

//Volver a la rama main y obtener los cambios guardados
$ git stash pop
```

# git cherry-pick
Este comando nos permite es tipo como un git merge pero especifico, eso porque podemos extraer un commit especifico de una rama alterna a la rama principal.

```js
//Cambiamos de rama
$ git switch 'rama-alterna'

//Hacer un cambio y un commit

//Volvemos a la rama principal y vemos la lista de commits
$ git switch main
$ git log --oneline
| * 65d37 (rama-alterna) cambio hecho en rama alterna
| * c3828 soy un commit de la rama principal

//Podemos traer ese cambio hecho en la rama alterna a la rama principal mediante el hash
$ git chery-pick 65d47
```
Con esto ya habremos traido ese commit pero se duplicara, tranquilo podemos cambiar el commit con un comando ya viste anteriormente, me refiero al ``git commit --amend``.

## #Dia14LearningGit