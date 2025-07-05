## Apuntes de comandos git

## Configuracion de usuario local
git config --global , configuracion global para la maquina local
    user.name"<>"
    user.email"<>"

git init , iniciar repositorio git en directorio raiz

git add <> , añadir ficheros para hacer commit

git commit -m "<>" , hacer fotografia, guardar cambios

git status , estado de los ficheros: con cambios, pendientes de añadir

git log , linea de commits hechos en la rama

git reset fichero, reset/quitar cambios añadidos al stage con git add

git checkout fichero/hash/tag , reset cambios del fichero al ultimo commit, desplazmiento al estado del commit usando el hash o su tag

.gitignore , archivo deode se especifican los ficheros para ignorar del reporsitorio

git reset --hard <hash> , remover/devolver commits a la rama main

git tag <name_n>, etiquetar un commit con un nombre, tag en donde se ubica el head

git tag, listado de tags

git branch <>, crear nuevo flujo

git switch <>, cambiar a otro flujo con nombre <>

git merge , combinar ficheros de un flujo a otro

git branch -d <flujo>, eliminar una rama
- al eliminar se quita la referncia a la rama/flujo pero todos los commits siguen exitiendo y son solo acessibles por su hash
- limpia el log para simplificar el arbol del proyecto

git stash, guardado temporal (WIP) sin hacer commit en la rama

git stash list, listar todos los stash

git stash pop, recuperar ficheros del guradado temporal

git stash drop, eliminar lista de stash

git reflog, log completo de aciones

## comandos para interactuar entre fiheros locales y github
### subir ficheros locales a github por primera vez
git remote add origin <> , asociar repositorio local con un reporitorio en github

git push -u origin main , enviar ficheros a un nuevo repositorio github

git fetch , descargar solo los cambios del arbol de commits

git pull , decargar ficheros del reporsitorio en github

git push , subir cambios a github

