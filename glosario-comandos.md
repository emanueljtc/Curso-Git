#GLOSARIO DE COMANDOS
1. git init  -> Crear Repositorio Actual (Local) e instala todo el                               funcionamiento de git para comenzar a trabajar. 
2. git clone direcciónURL -> Clona un repositorio remoto ya existente.
3. git add nombreArchivo[.] -> Agrega al repositorio los archivos que se le                                     indiquen.
4. git commit -m "mensaje" o -am "mensaje" + archivos -> texto descriptivo de                               los cambios aplicados al archivo.
5. git rm [archivo] -> elimina un archivo del area de trabajo y del staged
 5.1 git rm [archivo] -f -> forzar el borrado del archivo
 5.2 git rm --cache [archivo] -> Utilice esta opción para eliminar y eliminar             trazados solo del índice. Los archivos de árbol de trabajo,                    modificados o no, se dejarán solos.
6. git mv origen destino -> mover el archivo del origen al destino que queremos
7. git status -> Estado actual del arbol de trabajo local
8. git diff -> muestra diferencia entre los cambios en el estado local que aun                  no estan en el staged area.
  8.1 git diff --staged -> ampliación del anterior para mostrar diferencias con     un archivo ya subido al staged area o staged index
  8.2 git diff [branch 1] [branch 2] -> muestra la diferencias entre dos ramas.
9. git log -> muestra el log del commit es decir la información que compromete      a una rama de trabajo.
  9.1 git log [desde [..hasta]] --stat -s 'pattern'
10. git show [commit] -> ver un commit en especifico
11. git reset HEAD nombreArchivo -> marca el archivo para no ser incluido en el                                     proximo commit
12. git reset --soft HEAD -> desace el commit y conserva los cambios en el                                   arbol de trabajo local.
13. git reset --hard HEAD -> restablece el arbol de trabajo a la version del                                 ultimo commit.
14. git clean -> elimina los archivos desconocidos del arbol de trabajo local.

15. git checkout rama -> usado para diferentes acciones : recuperar archivos y commits, para hacer commits para crear y moverse entre los branch, etc
16. git branch -> lista las ramas locales si se le añade -f rama rev                  sobrescribe la rama existente y comienza antes de la revision
17. git merge ->  se utiliza para combinar dos ramas.

18. git pull -> descarga y guarda los cambios almacenados en el repositorio                     remoto.
19. git push [alias] [branch] -> sube los cambios a un repositorio remoto.
20. git fetch -> trae cambios desde un repo remoto pero no los fuciona para ellos abria que hacer merge.
21. git remote -> lista los repositorios remotos disponibles
22. git remore add [URLrepo] -> añade un repositorio remoto a la lista de repos                                 registrados.
23. Banderas: Son Iniciales que nos muestran lo que ocurre en nuestros archivos     y estado en que se encuentran en el momento. 
        M: Modified, A: Added, C: Copy-edit, D: Deleted, R: Rename-edit, 
        U: Unmerged