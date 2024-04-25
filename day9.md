# github, crear repositorio y configuracion:
antes que nada que es github, es una plataforma en la nube que permite a diferentes desarrolladores almacenar y administrar codigo.

## para empezar
- creamos una cuenta en la pagina oficila de github: ``https://github.com``.

### opcional
- Le damos click a nuestra foto por defecto.
- Editamos nuestra informacion ``edit profile``.
- Agregamos nuestro nombre, bio, redes.

## crear y configurar repositorio
- Le damos a la opcion ``+`` o ``new repository`` para crear un repositorio.
- Le damos un nombre.
- Configuramos si queremos el repositorio publico o privado.
- Agregamos un README.md y le damos a ``create repository``.

## vincular con nuestro 
- Le damos a ``<> code`` y copiamos la url http de nuestro repositorio.

- Lo clonamos para poder trabajarlo de manera local, realizamos esta sintaxis:
```js
//Clonar nuestro repositorio en nuestra maquina local
$ git clone https://github.com/{YOUR_USERNAME}/{YOUR_REPO}.git
```
- Con esto ya tendriamos el repositorio remoto de github en nuestro maquina local.
####  OJO: Ten en cuenta crear un token por seguridad

### empujar archivos a nuestro repositorio remoto
Podemos empujar``push`` a github debemos darle un push despues hacer los cambios y comitear nuestros archivos.
```js
//Pushear nuestros archivos comiteados a github
$ git push
```
Despues de esto todos nuestros cambios se subiran y ya habremos subido un archivo a github.

## #Dia9LearningGit