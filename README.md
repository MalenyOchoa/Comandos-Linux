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

- `git --help` // sirve para ver que opciones tengo y como se usan, se puede usar despues de un comando para ver como funciona
- `git init` //sirve para crear/inicializar un repositorio nuevo
- `git clone`//sirve para clonar un repositorio remoto: git clone *repo* *dir*
- `git status` // sirve para mostar el estado del repositorio
- `git add` //sirve para pre-confirmar un archivo (de rojo a verde): git add README.md
- `git diff` //sirve para mostrar los cambios en un archivo versionado(solo sirve si esta en rojo)
- `git commit` //sirve para confirmar los cambios en area de trabajo(lo que esta verde): git commit -m "mensaje"
- `git log` //sirve para mostar el historial de confirmaciones, +opcional: --graph --decorate --date-order --all
- `git push`//sirve para subir mis cambios locales a un repositorio remoto: git push "dondeguameter" "branchqueguasubir"
- `git remote`//sirve para mostrar los repositorios remotos que tengo de mi proyecto




-------------------------------------------------------------------------------



# COMANDOS PARA MYSQL

- //Para conectarse a una base de datos local
mysql -u usuario -p
(En terminal linux: No es necesario estar en un punto estrategico
o ruta establecida para poder acceder al servidor de bases de datos)

- //Mostrar bases de datos 
SHOW DATABASE;

- //Para abir/seleccionar una base de datos
Use nombre_bd;

- //MOSTRAR TABLAS
SHOW TABLES;