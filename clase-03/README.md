# Clase 03

## GIT RAMAS (Branchs) - REPASO

> Crear una rama
    git branch <nombre-rama>

> Moverme entre ramas
    git switch <nombre-rama>

> Para ver las ramas
    git branch

> Para borrar una rama
    git branch -d <nombre-rama>

> Para forzar el borrado de una rama
Recordar que este flag me sirve para confirmar el borrado de una rama que no fue fusionada con ninguna otra.
    git branch -D <nombre-rama>

## GIT MERGE (Fusiones)
Combinar los cambios de una rama con otra. Normalmente en un nuevo commit
**IMPORTANTE:** Tengo que estar en la rama que espero traerme los cambios. Es decir si quiero traer los cambios de dev a master
                debo estar sobre la rama master y ejecutar el siguiente comando
    git merge <nombre-rama>

### Abortar la fusion (merge)
    git merge --abort

### Tipos de Fusiones/Merge 
* Fast-forward (Union Automatica) GIT no necesita de la asistencia del usuario.
* Recursivo (Union Automatica) Tampoco hay conflictos.
* Manual (Conflictos) Ocurre cuando hay modificaciones en las mismas lineas de un archivo o varios archivos.

# Hola soy una linea que pronto se convertira en un conflicto (rama master)