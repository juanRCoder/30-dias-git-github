# Repaso y ejercicios de comandos basicos en git y github(2/5)

## Ejercicios:
### 1. Configuracion inicial
Configura tu nombre y correo electronico en git.
```js
//Configuracion para el usuario
$ git config --global user.name 'juanRCoder'
//Configuracion para el correo
$ git config --global user.email 'correo@gmail.com'
```

### 2. Subir archivos al repositorio.
Crea un repositorio llamadao `git-worshop` dentro de el crea un `README` y un archivo `file.txt`, luego de eso subelo al area de staged y comitealo.
```js
//Crear repositorio o directorio por ahora
$ mkdir git-workshop
//Adentrarse y subir agregar archivos
$ cd git-workshop/
$ echo 'esto es readme' > README.md
$ echo 'esto es un archivo txt' > file.txt
//Subir al area de staged y comitear
$ git add git-workshop/README.md git-workshop/file.txt
$ git commit -m 'add: up main files'
```

### 2. Correciones basicas
Si tu nombre no es `Hernán`, cambia el nombre del archivo Hernan.txt para que coincida con el tuyo. Por ejemplo, renómbralo a `<tu-nombre>.txt`, como `Pablo.txt`.
Reescribe el commit realizado en el paso anterior con el nuevo nombre del archivo.
```js
//Verifica que nombre tiene mi archivo con el comando de listado
$ ls
file.txt
//Cambiar el nombre del archivo
$ mv file.txt juanRCoder.txt
//Reescribimos el commit
$ git add juanRCoder.txt
$ git commit --amend -m 'esto es el nuevo commit reescrito'
```
### 3. Crear ramas:
Crea la rama “yo++” y cámbiate a esa rama, escribe una o dos oraciones acerca de ti en el archivo .txt con tu nombre, agrega tus cambios al área de preparación y realiza un commit.
Regresa al primer commit del repositorio usando git checkout master, crea otra rama llamada “taller-info” y cámbiate a esa rama.
En el archivo README.md, escribe una o dos oraciones acerca del taller.
Agrega los cambios al área de preparación y realiza un commit.
```js
//crear la rama y hacer los commit en la rama
$ git switch -c 'yo++'
$ echo 'oracion 1 y oracion 2' > juanRCoder.txt (yo++)
$ git add juanRCoder.txt (yo++)
$ git commit -m 'cambios en la rama yo++'(yo++)
$ git switch main
// crea otra rama llamada `taller-info` y hhacer los commit en esa rama
$ git switch -c 'taller-info'
$ echo 'oracion 3 y oracion 4' > README2.md (taller-info)
$ git add README2.md
$ git commit -m 'cambios en la rama taller-info' (taller-info)
$ git switch main
//Union de ramas
$ git merge taller-info
$ git merge yo++
```