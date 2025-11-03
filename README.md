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

##Como crear un conflicto
Para que haya un conflicto deben haber dos nuevos commits en cada rama que modifiquen el mismo archivo y que se fusionen 
Como se consige:
1 Crea una nueva rama
2 Haz cambios y commitealos
3 muevete a otra rama (puede ser la rama main o otra rama que parta del mismo punto que la rama modificada)
4 Haz cambios sobre el mismo archivo en la misma linia y commitealos
5 Al hacer merge hay un commit nuevo en cada rama que modifica lo mismo (la misma linia de un archivo) y git no sabe con cual quedarse
6 Tienes el conflicto

7 Para arreglarlo modifica el archivo desde la rama que recibe el merge y deja lo que quieras del archivo, 
finalmente haz git merge --continue o git add de los archivos modificados y un nuevo commit


#Ver cambios
git log --oneline
git show  --name-only

#Subir commit desde una rama que esta en local pero no en remoto
git push -u origin nuevaRama
