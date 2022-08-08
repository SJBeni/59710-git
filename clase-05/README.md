# Clase 05

## GIT RESET
### GIT Reset soft
    git reset --soft <hash>

### GIT Reset mixed
    git reset <hash>
    git reset --mixed <hash>
    
### GIT Reset hard (Peligroso)
Pierdo lo que tenia dentro de los commits. Es destructivo
    git reset --hard <hash>


## Trabajar en proyectos Open Source (Pull Request)

1. Hacer un fork del proyecto. Del proyecto del cual quiero contribuir (Debo copiar en mi cuenta el repo del proyecto original)
2. Me clono el fork desde mi cuenta de github
3. Trabajo normalmente. Subo los cambios (A mi propio repo)
4. Me voy al proyecto original, en el apartado Pull Request. Creo un nuevo pull request. Algunas veces aparece en mi repo la posibilidad de "Comparar
    y hacer Pull Request"
---
5. Si el repo original sufrio mas modificaciones (commits) voy a tener que actualizar mi repo fork.
6. Voy a la cuenta del proyecto original y me copio la url del repositorio
7. Agrego en mi repositorio local, la url (el remoto) del proyecto original
        git remote upstream <url-repositorio-original>
8. Me traigo los cambios del repositorio original a mi repo local
        git pull upstream <rama-que-quiero-actualizar>
9. Subo a mi repositorio remoto (Fork) las actulizaciones del repo local
        git push origin <rama-a-actualizar>

## Apuntadores

> Apuntadores dinamicos
* HEAD
> Apuntadores estaticos
* RAMAS (Locales y remotas)
* TAG
* STASH

## TAGs
> Listar TAGs
    git tag

> Crear TAG
    git tag <nombre-tag>

> Borrar tags
    git tag -d <nombre-tag>

> Crear tag con versionado semantico
    git tag -a v1.0.0 <hash> -m "Version 1.0.0"

* a: anotado
* m: mensaje

> Ver detalle de los tags, quien creo y en que commit estan creados
    git show <nombre-tag>

> Para subir tags especifico (Recomendado)
    git push origin <nombre-tag>

> Para subir todos los tags (NO recomendado)
    git push --tag
