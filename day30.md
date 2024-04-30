# Ejercicio Final - Git&Github(5/5)

## Ejercicio:
Crea un repositorio en GitHub llamado "MiProyectoWeb".
Clona el repositorio en tu computadora.
Crea una rama llamada "desarrollo" y cámbiate a ella.
Crea una estructura básica para un proyecto web dentro del repositorio (por ejemplo, carpetas para HTML, CSS y JS).
Crea un archivo HTML llamado "index.html" y añade un esqueleto básico.
Agrega estilos básicos al archivo CSS.
Haz tu primer commit con estos cambios.
Fusiona la rama "desarrollo" con la rama principal (usualmente llamada "main" o "master").
Sube los cambios a GitHub.
Configura GitHub Pages para que muestre tu proyecto web.
Haz cambios adicionales en tu proyecto (por ejemplo, añade más páginas, funcionalidades, estilos, etc.).
Haz commit de estos cambios y súbelos a GitHub.



```js
//1. Creamos un nuevo repositorio en github a travez de `new repository`.

//2. Clonames el repositorio en git
$ git clone https://TOKEN@github.com/USERNAME/REPO.git                

//3. Creamos una rama de desarrollo.
$ git switch -c 'desarrollo'

//Creamos los archivos basicos para construir en la web.
$ touch index.html styles.css script.js

//Agregamos la estructura los estilos y el codigo javascript

//Subimos nuestros cambios a github
$ git add index.html styles.css script.js

//Comiteamos nuestos cambios
$ git commit -m 'agregando estructura web'

//Pusheamos el proyecto
$ git push origin main
```

Creamos una accion automatizada para subirlo a github pages despues del git push

### Archivo yml
```yml
name: Deploy to GitHub Pages

on:
  push:
    branches:
      - main

jobs:
  deploy:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout code
        uses: actions/checkout@v2

      - name: Deploy to GitHub Pages
        uses: peaceiris/actions-gh-pages@v3

        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./
```

Listo con esto cada vez que haga push , se desplegaria a github pages con la instruccion dada.

Esto es lo ultimo del reto de 30 dias de git y github, feliciadades si alcanzaste el reto o llegaste a este punto, logramos un objetivo y es aprender git y github de apocos pero entendimos.

## #Dia30LearningGit