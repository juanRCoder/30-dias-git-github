# Modificar y deshacer commits:
Aprendamos un poco a controlar lo scommit antes de pushearlos o subirlos a un servidor.

Para este ejercico hagamos 5 commits  para ver:
```js
// Ver listado de commits
git log --oneline

50500 (HEAD -> main) quinto commit //-> commit actual
f22c4 cuarto commit
12c4f tercero commit
a22g4 segundo commit
68e7e primero commit

//Agregar un nuevo cambio pero no quiero otro commit
git commit --amend 

//retrocer un commit atras
git reset --soft f22c4

//comprobar
git log --oneline

50500 (HEAD -> main) cuarto commit //-> commit actual
12c4f tercero commit
a22g4 segundo commit
68e7e primero commit

//restablecer un archivo a un commit anterior
$  git reset --hard 12c4f

//comprobar
git log --oneline

12c4f (HEAD -> main) tercero commit //-> commit actual
a22g4 segundo commit
68e7e primero commit
```
OJO: Cada vez que haces un cambio de commit guardalo y no dejes nada sin guardar porque puede haber conflictos.

## #Dia5LearningGit