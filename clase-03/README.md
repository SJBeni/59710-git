# CLASE 03
## GIT RAMAS (Branchs) - REPASO
> Crear una rama
    git branch <nombre-rama>

>Moverme entre ramas
    git switch <nombre-rama>

> Para ver las ramas
    git branch

> Para borrar una rama
    git branch -d <nombre-rama>

> Para forzar el borrado de una rama
    Recuerden que este flag me sirve para confirmar el borrado de una rama que no fue fusionada con ninguna otra
    Git realiza esa advertencia para evitar que se borre una rama que no fue mergeada, por error
        git branch -D <nombre-rama>
        