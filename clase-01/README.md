# Clase 01

## COMANDOS DE CONSOLA BASICOS

* ls : listar directorios

* cd : cambiar direcotorio
    cd <directorio>
    ejemplo : cd clase-01

* cd .. : salir de un directorio

* touch : creacion de archivos vacios
    touch<nombre-archivo>
    ejemplo : touch archivo1.txt

* mkdir : crear directorios
    mkdir<nombre-directorio>
    ejemplo : mkdir dir1 dir2

* rm : borra archivos
    rm<archivo-a-borrar>
    ejemplo : rm index.html

* rmdir : borrar un directorio
    rmdir<directorio-a-borrar>
    ejemplo : rmdir dir1

* clear : limpio la consola

## GIT

> Saber si tengo GIT instalado
    git --version

> Configuracion importante de GIT
  GLOBAL: Para todos los repositorios que se creen en el equipo

    git config --global user.name "nombre"
    git config --global user.email "correo"

> Inicializar repositorio git (Crear un repositorio)
    git init

> Configuracion importante de GIT
  LOCAL: Para el repositorio actual, configuro usuario y correo

    git config --local user.name "nombre"
    git config --local user.email "correo"

### GIT STATUS
    Me permite ver los cambios que tengo en el Working Directory (WD) respecto del Repositorio
        git status

### GIT ADD
    Me permite agregar archivos al temporal de confirmacion de cambio. Siempre tengo que hacer esto cada vez que quiero sacar una foto (commit)
    Mueve los archivos del WD al Staging Area (Index)
        git add .

### GIT COMMIT
    Sacar la foto, colocar lo que tenia en el Staging Area en el repositorio
        git commit -m "Mensaje"

### GIT LOG
    Muestra las fotos o los commits que tengo en el repositorio
        git log