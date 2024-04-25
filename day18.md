# git flow
Es un manejo de aplicacicones en el cual manejar el proyecto en diferentes etapas de manera ordenada y profesional segun yo.

Cuando incializamos nos crea una rama ``develop`` donde a partir de ahi podremos trabajar en diferentes ramas o grupos de trabajo.

## Pasos para iniciar
1. Inicializamos un repositorio
<br/>``git init``
2. Incializamos git flow
<br/>``git flow init``

Ramas especiales para diferentes etapas o cambios en el proyecto.

## branchs feature, release, hotfix

### feature
Rama para agregar o cambiar una nueva caracteristica del proyecto.
```js
//Creamos una caracteristica(feature)
$ git flow feature start (name-feature)

//Luego seremos trasladado a la rama creada 

//Hacemos todos los cambios lo agregamos a stage y lo comitemaos

//Despues de eso cerramos y lo mergeamos con la rama develop
$ git flow feature finish
```


### release
Rama para desplegar una nueva version del proyecto a produccion
```js
//Creamos un despliegue(release)
$ git flow release start (name-release)

//Luego seremos trasladado a la rama creada 

//Hacemos todos los cambios lo agregamos a stage y lo comitemaos

//Despues de eso cerramos y lo mergeamos con la rama develop
$ git flow release finish
```

### hotfix
Rama para cambiar o agregar un cambio en caliente en produccion.
Estas correcciones se aplican a problemas críticos que necesitan ser solucionados de inmediato, como errores que afectan la funcionalidad del software en producción o vulnerabilidades de seguridad importantes.
```js
//Creamos una arreglo(hotfix)
$ git flow hotfix start (name-hotfix)

//Luego seremos trasladado a la rama creada 

//Hacemos todos los cambios lo agregamos a stage y lo comitemaos

//Despues de eso cerramos y lo mergeamos con la rama develop
$ git flow hotfix finish
```