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
    Los archivos que quiero hacer commit deben estar en seguimiento. O sea, no ser Untracked (Archivos que no estan en seguimiento), ya que no los va a agregar el git add
    git commit -am "Mensaje"

### Para enmendar un commit
Agrego los archivos que faltaron en el ultimo commit utilizando: git add <archivo>
Luego ejecuto:
    git commit --amend
OBS: para modificar el mensaje, se abre la consola, en este caso, gitbash
     para guardar los cambios y salir de esa ventana, ejecutar la combinacion
            Esc + Shift + Z + Z
     de esta forma, el amend termina, habiendose modificado el commit

## Status de Archivos

* Untracked: Archivos que no se agregaron al index (Staging Area), es decir archivos que estan en el Working Directory
* Unmodified: Son archivos que ya estan en el repositorio, es decir ya tienen una foto (commit)
* Modified: Son archivos que ya estan en el repositorio, pero con respecto al Working Directory tienen modificaciones 
            detectadas por git (compara la foto del repositorio con el WD)
* Staged: Archivos que estan confirmados para ser un proximo commit

## GIT LOG
>Mostrar la documentacion de un comando en particular
    git log --help
>Muestre los commit en una cantidad especifica
    git log -2
> Muestre los commit por fecha y sus variantes
    git log --since="2022-05-01"
    git log --after="2022-05-01"
    git log --before="2022-05-01"
    git log --after="2022-05-01" --before="2022-05-10"
    
## GIT RAMAS (Branchs)
> Crear una rama
    git branch <nombre-rama>

> Moverme entre ramas
    git switch <nombre-rama>

> Para ver las ramas
    git branch