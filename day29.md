# Repaso y ejercicios de comandos basicos en git y github(4/5)

## Ejercicio:
### Cambios en los commits
Mostrar los cambios de la última versión del repositorio con respecto a la anterior.
Cambiar el mensaje del último commit por “Añadido capítulo 3 sobre gestión de ramas al índice.
```js
//Mostrar el historial de commits de nuestro repositorio
$ git log --oneline
bd75c (HEAD -> main, origin/main, origin/HEAD) Merge pull request #1 from juanRCoder/features/auth1
5e8bd (origin/features/auth1, features/auth1) Realizando una commit en una rama
9a900 Day27: Repaso y ejercicios de comandos basicos en git y github (2/5)
fa856 Merge branch 'taller-info'
98d9c Merge branch 'feature/exercises1'
d5544 cambios en la rama taller-info

//Retroceder un commit anterior para deshacer un cambio
$ git reset --hard 5e8bd
5e8bd (origin/features/auth1, features/auth1) Realizando una commit en una rama

//Luego actualizar el commit con los nuevos cambios incorporados por 'Anadiendo capitulo 3 de ramas al indice'
$ git add .
$ git commit --amend -m 'Anadiendo capitulo 3 de ramas al indice'
$ git push
```

## #Dia29LearningGit