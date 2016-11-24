
# COMANDOS LINUX

//Ctrl + Alt + T  -> Abre terminal
```bash

--help  #sirve para ver opciones tengo y para que sirven

cd      #sirve para moverme entre carpetas

cd ..   #sirve para retroceder al directorio anterior

pwd		#sirve para saber en que directorio estoy

ls      #sirve para ver lo que hay dentro de un directorio

ls -l  	#sirve para ver los archivos en forma de lista

ls -a   #sirve para ver los archivos ocultos

cat     #sirve para ver que hay dentro de un archivo/doc

mkdir	#sirve para crear un nuevo directorio

nano	#sirve para crear/editar/modificar archivos: nano *nombrearchivo*

mv 		#sirve para mover/renombrar un archivo: mv *nombre* *nuevonombre*

cp 		#sirve para copiar un archivo: cp *rutaActual* *rutaDondeDeseaCopiar*

rm 		#sirve para remover/eliminar un archivo: rm ~/*ruta*


```


--------------------------------------------------------------------------------



# COMANDOS DE GIT

- `git --help` //sirve para ver las opciones y como se usan,Se puede usar despues de un comando para ver como funciona
- `git init` //sirve para crear/inicializar un repositorio nuevo
- `git clone`//sirve para clonar un repositorio remoto: git clone "repo" "dir"
- `git status` // sirve para mostar el estado del repositorio
- `git add` //sirve para pre-confirmar un archivo (de rojo a verde): git add README.md
- `git diff` //sirve para mostrar los cambios en un archivo versionado(solo sirve si esta en rojo)
- `git commit` //sirve para confirmar los cambios en area de trabajo(lo que esta verde): git commit -m "mensaje"
- `git log` //sirve para mostar el historial de confirmaciones, +opcional: --graph --decorate --date-order --all
- `git push`//sirve para subir mis cambios locales a un repositorio remoto: git push "dondeguameter" "branchqueguasubir"
- `git remote`//sirve para mostrar los repositorios remotos que tengo de mi proyecto

# TRABAJAR CON REMOTOS
Para poder colaborar en cualquier proyecto Git, necesitas saber cómo gestionar repositorios remotos.
Los repositorios remotos son versiones de tu proyecto que están hospedadas en internet en cualquier otra red.
Gestionar un repositorio remoto incluye saber cómo añadir un repositorio remoto, eliminar los remotos que ya no son válidos,
gestionar varias ramas remotas y definir si deben rastrearse o no, y más.

#- * VER TUS REMOTOS *

Para ver los remotos que tienes configurados, debes ejecutar el comando `git remote`
Mostrará los nombres de cada uno de los repositorios que tienes especificados. Si has clonado tu repositorio, deberías ver
almenos `origin` - este es el nombre que por defecto Git le da al servidor del que has clonado:

```
$ git clone http://github.com/MalenyOchoa/nombreRepositorio.git
.................
.............
...........
$ cd nombreRepos
$ git remote
origin

```
También puedes pasar la opcion `-v`, la cual muestra las URLs que Git ha asociado al nombre
y que serán usadas al leer y escribir ese remoto:


``

$ git remote -v

origin https://github.com/MalenyOchoa/nombreRepo.git  (fetch)
origin https://github.com/MalenyOchoa/nombreRepo.git (push)

``

Si tienes más de un remoto, el comando los listará todos.


#- * AÑADIR REPOSITORIOS REMOTOS *

Para añadir un remoto nuevo y sociarlo a un nombre que puedas referenciar fácilmente,
ejecuta:

 `git remote add [nombre] [url] `:


```
$ git remote
origin
$ git remote add repoMaleny https://github.com/MalenyOchoa/nmbRepositorio.git
$ git remote -v
origin     https://gith..... (fetch)
origin     https://gith..... (push)
repoMaleny https://gith..... (fetch)
repoMaleny https://gith..... (push)

```

A partir de ahora puedes usar el nombre `repoMaleny` en la linea de comandos en lugar de la URL entera.
por ejemplo, si quieres traer toda la información que tiene MalenyOchoa pero tu aun no tienes en tu repositorio,
puedes ejecutar `git fetch repoMaleny`

#- * ENVIAR TUS REMOTOS *

Cuando tienes un proyecto que quieres compartir, debes enviarlo a un servidor.
el comando para hacerlo es: `git push [nombre-remoto] [nombre-rama]`.
Si quieres enviar tu rama `master` a tu servidor `origin` 
(Recuerda, clonar un repositorio establece esos nombres automaticamente)
puedes ejecutar el siguiente comando y se enviarán todos los commits que hayas hecho al servidor:


``

$ git push origin master

``

#- * ELIMINAR Y RENOMBRAR REMOTOS *

- Si quieres cambiar el nombre de la referencia de un remoto, puedes ejecutar `git remote rename`.
Por ejemplo, si quieres renombrar `repoMaleny` a `repoM`, puedes hacerlo con `git remote rename`:

``

$ git remote rename repoMaleny repoM
$ git remote
origin
repoM
``

- Si por alguna razón quieres eliminar un remoto, puedes utilizar `git remore rm`:


``

$ git remote rm repoM
$ git remote
origin

``








-------------------------------------------------------------------------------



# COMANDOS PARA MYSQL

- //PARA CONECTARSE a una base de datos local:  
mysql -u usuario -p    #(En terminal linux: No es necesario estar en un punto estrategico
o ruta establecida para poder acceder al servidor de bases de datos).

- //MOSTRAR bases de datos:   
SHOW DATABASE;

- //Para ABRIR/SELECCIONAR una base de datos:  
USE nombre_db;

- //MOSTRAR Tablas:
SHOW TABLES;
