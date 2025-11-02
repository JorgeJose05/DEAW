# Ejercicio 1

para configurar nombre, y email es

git config user.name "Nombre"
git config user.email "email"

Para imprimirlo es:

git config user.name
git config user.email

Para ver los cambios entre la rama actual y la main usa:

git diff

(Te da los archivos y los cambios que se han hecho)

##Como se elimina una rama	
git branch -d nombreDeLaRama

##Como fusionar una rama
git merge nombreDeLaRamaAFusionar -m "Mensaje del merge. Se merge desde la rama que quieres que tenga los nuevos cambios"
