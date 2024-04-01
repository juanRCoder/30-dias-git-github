# Concepto e Instalacion de Git

- GIT es un sistema de control de versiones distribuido que permite gestionar diferentes versiones de un archivo.

- Podemos ver los diferentes cambios de un archivo, quien hizo cambios anteriores, un historial de diferentes cambios, y asi mantener un registro o trabajar en un archivo que esta siendo utilizado por otro al mismo tiempo.


## Instalacion
1. Buscar en google 'descargar git' - (Git - Downloads).
2. Descargar segun su sistema operativo.
3. Le dan a todo next -> next y next.
4. Listo ya descargaste git bash, que es la terminal de git.

## Configuracion
- Definir el gmail y username para decirle a git quien hace los cambios.
```js
//Configuracion global para el usuario.
git config --global user.name "usuario1"

//Configuracion global del correo
git config --global user.email "usuario1@gmail.com"
```

- Para ver las configuraciones hacer lo siguiente.
```js
//Ver configuraciones globales
git config --global --list
o
//Ver todas las configuraciones
git config --list
```

* Tambien podemos ver la lista de todos los comandos que iremos viendo con calma en estos dias
```js
//Ver comandos de git
git help
```