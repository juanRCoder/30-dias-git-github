# Git restore, git reset y git checkout.
Comprendamos un poco mas sobre los cambios en el stage y la restauracion de archivos.

## Git restore
Este comando me permite a mi restaurar archivos al ultimo cambio que tengo, supongamos que tengo un archivo el cual modifico para obtener otro texto, al igual que un archivo tambien puedo recuperar un directorio.
```js
//Archivo antes de modificar
$ cat archivo.txt
|
L 'texto del archivo'

//Modificar el archivo.
$ echo 'cambiando el archivo' > archivo.txt

//Recuperar el contenido del texto del ultimo cambio.
$ git restore archivo.txt

//ahora tengo el texto anterior al cambio.
$ cat archivo.txt
|
L 'texto del archivo'
```
Al igual que un texto tambien puede funcionar con directorios.

## Git reset
git reset me permite recuperar archivos o directorios de la zona de stage(antes de hacer commit).

```js
//Agregar archivo a la zona de preparacion(stage)
$ git add archivo.txt

//Vemos los archivos en la zona de stage
$ git status
L 'modified: archivo.txt'

//Reseteamos ese archivo que no queremos subir
$ git reset archivo.txt

//Verificamos nuevamente para ver que no haiga nada agregado.
$ git status
L 'void' -> explico que esta vacio
```

## Git checkout
Tambien podemos restaurar un archivo de un commit en especifico de una version anterior del archivo en particular esto a travez de este comando.

```js
//Archivo antes de modificar
$ cat archivo.txt
|
L 'texto del archivo'

//Cambiamos el archivo a un version en especifica mediante el ID del commit.
$ git checkout 123456 archivo.txt

//ahora tengo el texto del commit en especifico.
$ cat archivo.txt
|
L 'texto del archivo commit1'
```

* Con el `git checkout` tambien podemos cambiar entre ramas pero eso se explicaraen otro dia.
## #Dia3LearnGit