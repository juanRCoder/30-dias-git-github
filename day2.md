# Uso básico de Git
Algunas ventajas de usar git:
1. Verificar historial.
2. Almacenar codigo.
3. Trabajar en equipo.
4. Saber cuando se introdujo un error.

Antes de poder manipular archivos y conocer algunos comandos basicos tengamos en cuenta algo que debemos dejarlo claro.

## Diferencia entre repositorio y directorio.
- un repositorio es como una libreria puede almacenar cantidades de archivos, carpetas, multimedia, entre otros, asi como vez en github.

- por otro lado un directorio es simplemente una carpeta el cual pueedes colocar archivos y eliminar archivos.

```js
- CursoGit/ //-> repositorio
    - historiaGit/ //-> directorio
        - script.js

    - comandosGit/ //-> directorio
    - comandosGit2/ //-> directorio
    - img.webp 

```

## Comandos basicos de git 
Estos comandos basicos de git te ayudaran a poder manipular, mover archivos, etc, comencemos:

```js
$ ls                       // -> listar archivos y carpetas del directorio actual.
$ pwd                      // -> mostrar la ubicacion actual del directorio.
$ cd ..                    // -> retroceder un nivel anterior de la carpeta actual.                    
$ cd historiaGit/          // -> acceder a un directorio(carpeta).
$ mkdir comandosGit/       // -> crear un directorio(carpeta).
$ rmdir comandosGit/       // -> eliminar un directorio.
$ git init                 // -> inicializar una carpeta a un repositorio.
$ git add comandosGit/     // -> agregar archivo para subirlo al repositorio.
$ git status               // -> mostrar los estados de los archivos.
$ git commit               // -> escribir un mensaje detallado en la ventana que aparece sobre el cambio.
$ git commit -m 'message'  // -> escribir un mensaje corto en (message) sobre lo realizodo.
```
## Flujo de git basico:
El flujo por el cual pasa el archivo o carpeta es el siguiente(<b>por ahora solo esto</b>).
<br/>
1. <b>git add</b> -> agregar el archivo a una area de preparacion.
2. <b>git status</b> -> verificar si el archivo esta agregado o no(<b>debe estar de color verde</b>).
3. <b>git commit -m 'first commit'</b> -> commitear el archivo listo para subirlo a github.


## #Dia2LearnGit