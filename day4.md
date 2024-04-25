# Git diff.
Git diff nos permite ver los cambios entre archivos, ver diferencias en el contenido y ver cambios entre commit especificos.

Antes tambien debemos conocer un comando llamado  `git log --oneline.`

```js
//Nos permite ver el listado de los commits realizados en el repositorio.
$ git log --oneline
//Example:
`
	41f9f6a (HEAD -> main) mensaje commit actual
	ce2cbd4 (origin/main, origin/HEAD) mansaje commit anterior
`

//Vemos la diferencia de un archivo en stage y uno comiteado
$ git diff --staged

//Ver la diferencia entre dos commits(antes debemos conocer el hash/ID del commit)
$ git diff 'commit1' 'commit2'

//Ver los cambios en el contenido del archivo
$ git diff --word-diff 'commit1' 'commit2'
```

## #Dia4LearningGit