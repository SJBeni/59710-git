# Clase 04

## GIT CHERRY PICK
**IMPORTANTE:** Tengo que estar ubicado en la rama que espero traerme el o los commits.
    git cherry-pick <hash>
    git cherry-pick <hash1> <hash2> <hash3>

        git cherry-pick <hash>^..<hash> #Todos los commits incluidos en el rango y ademas los extremos

        git cherry-pick <hash>..<hash> #Todos los commits incluidos en el rango y sin los extremos
**Si tengo varios commits, no uno. Voy a tener que hacer**
    git cherry-pick --continue

## Para abortar el proceso de cherry-picking
    git cherry-pick --abort

## GIT ALIAS
    git config --global alias.ll "log --oneline --decorate --all --graph"
    git config --global alias.l "log --oneline"
    git config --global alias.s "status --short"

## Para listar alias
    git config --get-regexp alias

## Para quitar un alias
    git config --global --unset alias.<alias>
    
## GIT STASH
Es construido basado en una estructura de datos pila
>¿Que me permite el stash?
    Me permite registrar temporalmente los cambios de WD y Staging Area (SA).
    

### Crear un stash
    git stash