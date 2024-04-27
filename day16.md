# new commit, squash o rebase
Estas 3 opciones son las que nos ofrecen para aceptar o mejor dicho mergear un pull request de otro desarrollador.

## new commit
Esta es la primera opcion que nos permite crear un commit en el cual contenga todos los cambios que el desarrollador hizo para aportar en nuestro proyecto.
```js
Rama main:
         A --- B --- C --- M (main)

Rama feature:
             D --- E --- F (feature)
//Donde M es el nuevo commit de merge que fusiona los cambios de feature en main.
```

## squash
Este tipo de merge nos permite acoplar todos los commit hechos por el dev en uno solo para mergear al repositorio original.
```js
Rama main:
         A --- B --- C --- S (main)

Rama feature:
             D --- E --- F (feature)
//Donde S es un nuevo commit que contiene los cambios combinados de feature en uno solo.
```

## Rebase
Esta ultima opcion es diferente a los otros porque nos permite tener el historial de commit que realizo el desarrollador, asi tendremos un control de todos los cambios hechos por el en nuestro repositorio original.
```js
Rama main:
         A --- B --- C --- (D) --- (E) --- (F) (main)

Rama feature:
                  (feature)
//Donde D', E', y F' son los commits de feature reorganizados sobre main. La rama feature se "recoloca" sobre main.
```

## #Dia16LearningGit