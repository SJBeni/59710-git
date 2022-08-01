# Clase 04

## GIT CHERRY PICK
**IMPORTANTE** Tengo que estar ubicado en la rama que espero traerme el o los commits.
    git cherry-pick <hash>
    git cherry-pick <hash1> <hash2> <hash3>
    
```sh
    git cherry-pick <hash>^..<hash> #Todos los commits incluidos en el rango y ademas, los extremos
```
```sh
    git cherry-pick <hash>..<hash>  #Solo me trae los que estan entre esos 2 commits, no las puntas
```

### Si tengo varios commits, no uno. Voy a tener que hacer
    git cherry-pick --continue
### Para abortar el proceso de cherry-picking
    git cherry-pick --abort

## GIT ALIAS
### Para crear alias
    git config --global alias.<nombre-alias> "comando sin la palabra git"

### Para listar alias
    git config --get-regexp alias

### Para quitar un alias
    git config --global --unset alias.<nombre-alias>

## GIT STASH
 Es construido basado en una estructura de datos conocida como pila.
>¿Que me permite hacer el stash?
  Me permite registrar temporalmente los cambios del Working Directory y el Staging Area
>¿Puedo subir al remoto los stash?
  No. Solo estan en el repositorio local. No se pueden subri al remoto.

### Crear un stash
    git stash

### Listar los stash
    git stash list

### Recuperar los stash
**Nota** Si el stash que estoy tratando de recuperar genera un conflicto con mi codigo, o sea con el codigo que esta en el repositorio
         Me va a dejar en la caja el stash que estoy sacando. Si no hay conflictos, borra el stash actual de la pila.
         git stash pop

### Borrar el ultimo stash
    git stash drop
    git stash drop stash@{numero-stash}

### Si quiero aplicar un stash particular (solo aplica, no borra lo aplicado)
    git stash apply stash@{numero-stash}

### Si quiero aplicar un stash en una rama nueva
    git stash branch <rama-a-aplicar-stash>

## Versiones DESKTOP
* Git Kraken: https://www.gitkraken.com/
* Git Desktop: https://desktop.github.com/

## Buenas practicas para generar mensajes de commits
https://medium.com/@jmz12/buenas-pr%C3%A1cticas-para-commits-5eb4c86b9a47

