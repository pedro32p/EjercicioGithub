- En el paso 11 ejecuto el comando *git reset --hard HEAD~1* porque además de
deshacer el commit quiero que se modifique también el working copy.

- En el paso 12 ejecuto el comando *git reflog* para ver el identificador del 
commit que he perdido. Una vez que lo he encontrado ejecuto *git reset --hard
<identificador> para recuperar ese commit y para que el working copy también 
se modifique.

- En el paso 13 el *git merge master* que ejecuto no causa ningún conflicto
porque no hemos modificado git-nuestro.md en las dos ramas y en las mismas
líneas.

- El merge del paso 19 si que causa un conflicto porque el archivo 
git-nuestro.md ha sido modificado en ambas ramas y en las mismas líneas.

- El merge del paso 21 no causa conflicto ya que en la rama master el archivo
git-nuestro.md no había sido modificado.

- En el paso 25 utilicé los siguientes comandos:
   *git config alias.dibujaGrafo "log --graph --decorate --pretty=online"*
   *git dibujaGrafo

- El merge del paso 26 no podría ser fast forward ya que ambas ramas contienen
commits y por tanto no forman una lista.

- En el paso 27 utilicé el comando *git reset HEAD~1*.

- En el 28 descarto los cambios con *git checkout -- git-nuestro.md*.

- En el 29 elimino la rama con *git branch -D title*.

- En el paso 30 para rehacer el merge que he deshecho utilizo
*git reset --hard <indentificador>*.

- En el paso 32 ejecuto *git checkout <identificadorDelCommit>*.

- En el paso 33 ejecuto *git checkout <identificadorDelCommit>*.



 
