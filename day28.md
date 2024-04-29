# Repaso y ejercicios de comandos basicos en git y github(3/5)

## Ejercicios:
### 1. Flujo de trabajo con github flow
Actualiza tu repositorio base mediante una rama y manda un pull request para verificarlo con el equipo de trabajo.
```js
//Clonar repositorio
$ git clone https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/{YOUR_REPO}.git     

//Luego creamos una rama para trabajar en ella y hacer los cambios y subir la rama
$ git switch -c 'features/auth1'
$ echo 'console.log("Hola Mundo")' > server.js  (features/auth1)
$ git add server.js
$ git commit -m 'agregando un nuevo archivo server'
$ git push origin features/auth1

// Listo para hacer la pull requests
```