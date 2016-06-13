# GitNuestro-kw
Git nuestro :)
1. Deshacer un commit *perdiendo los cambios en el Working Copy*
- user$ git reset --hard HEAD~1 (Debido a que de este modo perdemos los cambios del Working Copy)
2. Rehacer el último commit *deshaciendo el que acabamos de deshacer*
- user$ git reflog (Nos muestra todos lo commits de nuestro repositorio y en orden desde más nuevo a más antiguo)
- user$ git reset --hard idCommit (volvemos a recuperar el commit perdido)
3. Hacer un merge con ‘master’ *styled absorbe a master*
- No, causa ningun conflicto ya que se ha modificado el archivo de la rama styled. Y la rama master absorbe la cambios realizados en la rama styled. 
4. Hacer un merge de “htmlify” en “styled” *styled absorbe a htmlify*
