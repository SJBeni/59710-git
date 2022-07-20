# CLASE 03
## GIT RAMAS (Branchs)
> Crear una rama
    git branch <nombre-rama>
>Moverme entre ramas
    git switch <nombre-rama>
> Para ver las ramas
    git branch
> Para borrar una rama
    git branch -d <nombre-rama>
> Para forzar el borrado de una rama
    Recuerden que este flag me sirve para confirmar el borrado de una rama que no fue fusionada con ningun otra
        git branch -D <nombre-rama>

## GIT MERGE

    git merge <nombre-rama>

### Tipos de Fusiones/Merge
* Fast-forward (Union Automatica) Git no necesita de la asistencia del usuario. Tampoco hay conflictos
* Recursivo (Union Automatica) Tampoco hay conflictos
* Manual (Conflictos) Ocurre cuando hay modificaciones en las mismas lineas de un archivo o varios archivos

## Esto es algo nuevo que tengo que probar. (origen: rama-conflicto)