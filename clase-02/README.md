# Clase 02

## GIT REMOTE

### Agregar remoto

    git remote add origin <URL>
    git remote add origin https://github.com/SJBeni/59710-git.git

### Verificar los remotos
    git remote
    git remote -v   #verbose: va a dar mas informacion del remoto

### Para subir el repo local al remoto
    git push -u origin master     ---> la primera vez

## GITIGNORE
    Me permite descartar archivos y carpetas que no quiero subir

## GITKEEP
    Me permite mantener y versionar carpetas vacias
    Esto fue creado por la comunidad, para resolver la necesidad de incluir carpetas vacias
    pero necesarias para la funcionalidad de un programa.
    No pertenece a la documentacion de git

## GIT COMMIT

### Para hacer un commit
    git commit -m "Mensaje"

### Para hacer un git add y un git commit en simultaneo
    Los archivos que quiero commitear deben estar en seguimiento. O sea, no ser Untracked (Archivos que no estan en seguimiento), ya que no los va a agregar el git add
    git commit -am "Mensaje"

### Para enmendar un commit
    git commit --amend

## Status de Archivos

* Untracked: Archivos que no se estan siguiendo. No fueron afectados por git add
* Modified: Son archivos que ya estan en el repositorio pero respecto al Working Directory

## GIT LOG
>Mostrar la documentacion de un comando en particular
    git log --help
>Muestre los commit en una cantidad especifica
    git log - 2
> Muestre los commit por fecha y sus variantes
    git log --since="2022-05-01"
    git log --after="2022-05-01"
    git log --before="2022-05-01"
    git log --since="2022-05-01" --oneline

## GIT RAMAS (Branchs)
> Crear una rama
    git branch <nombre-rama>
>Moverme entre ramas
    git switch <nombre-rama>