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