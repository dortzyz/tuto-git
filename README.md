## Apuntes de comandos Git

### Configuracion de usuario local
git config --global , configuracion global para la maquina local:
    user.name"nombre del autor"
    user.email"correo"

### Iniciar git

git init , iniciar repositorio git en directorio raiz.

#### Nombre de archivo para ignorar ficheros:
.gitignore , archivo donde se especifican los ficheros para ignorar del reporsitorio.

### Comandos mas usados

git add <> , añadir ficheros para hacer commit.

git commit -m "comentario para el commit" , hacer fotografia, guardar cambios.

git status , estado de los ficheros: con cambios, pendientes de añadir.

git log , linea de commits hechos en la rama.

git checkout <fichero/hash/tag> , restaurar cambios guardados del fichero al del ultimo commit, desplazamiento entre commits usando el hash o el tag.

git restore <fichero> , restaruar los cambios guardados del fichero que aun no sean añadido al stage (git add), comando nuevo separad de hit checkout.

git tag <name_n>, etiquetar un commit con un nombre, tag en donde se ubica el head.

git tag, listado de tags.

git branch <>, crear nuevo flujo.

git switch <>, cambiar a otro flujo con nombre <>.

git merge , combinar ficheros de un flujo a otro.

git branch -d <flujo>, eliminar una rama
- al eliminar se quita la referncia a la rama/flujo pero todos los commits siguen exitiendo y son solo acessibles por su hash.
- limpia el log para simplificar el arbol del proyecto.

### Comandos para guardar cambios sin lanzar commit

git stash, guardado temporal (WIP) sin hacer commit en la rama.

git stash list, listar todos los stash.

git stash pop, recuperar ficheros del guradado temporal.

git stash drop, eliminar lista de stash.

git reflog, log completo de aciones.

### Comando de git reset

git reset <fichero>, reset/quitar cambios añadidos al stage con git add.

git reset --hard <hash> , remover/devolver commits a la rama main.

## Comandos para interactuar entre ficheros locales y Github

### Subir ficheros locales a github por primera vez
git remote add origin <> , asociar repositorio local con un reporitorio en github.

git push -u origin main , enviar ficheros a un nuevo repositorio github.

### Comandos para sincronizar ficheros en Github

git fetch , descargar solo los cambios del arbol de commits.

git pull , decargar ficheros del reporsitorio en github.

git push , subir cambios a github.

