# Repaso y ejercicios de comandos basicos en git y github(1/5)
Bueno, entrando a la recta final de este reto de 30 dias de git and github hablemos un poco o resolvamos algunos ejercicios de git

## Ejercicios:
### 1. Inicializar un repositorio.
Inicializa un repositorio y subelo a la carpeta de github
```js
//Si ya tienes creado tu reposiotrio creado inicializalo.
$ git init
$ git remote add origin https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/{YOUR_REPO}.git    
$ git add .
$ git commit -m 'first commit'
$ git push        
```

### 2. Agregar y confirmar cambios
Crea un archivo , agregale contenido y luego agregalo a la zona de stage y confirma los cambios
```js
//Crear un archivo con contenido
$ echo "print('Hola Python')" > file.py

//Agregar a la zona de stage 
$ git add file.py

//Confirmar el cambio comiteando el archivo
$ git commit -m 'feat: add file.py'
```

### 3. Ver el historial de cambios y crear una nueva rama
Muestra el historial de commits del repositorio y crea una nueva rama del proyecto.
```js
//Ver el historial de commits del proyecto
$ git log --oneline
'''
65edc (HEAD -> main, origin/main, origin/HEAD) Day25: Github Pages & Github Actions
5ad0e Day24: Autenticacion repository with Token
a09c8 Day23: COnfiguracion  SSH con github y git
d8612 Day22: git fetch & git merge -> (git pull)
60c0e Day21: stage zone, commit and server github
b20b4 Day20: Git Flow vs GitHub Flow
62a76 Day19: Github Flow
'''
//Si quieres dejar de verlo apretar 'q'

//Crear una nueva rama
$ git switch -c 'nombre_rama'
//Comando para ver las ramas actuales
$ git branch
  feature/exercises1
* main
```

### 4. Realizar merge de ramas y deshacer cambios no deseados.
Realizar un merge de una rama alterna a la principal y saca archivos de la zona stage.
```js
//Vamos a la rama feature/exercises1 y comiteamos para el merge
$ git switch feature/exercises1
$ git add file.js
$ git commit -m 'cambios actualziados en la rama'
//Volvemos para el merge
$ git switch main
$ git merge feature/exercises1
```