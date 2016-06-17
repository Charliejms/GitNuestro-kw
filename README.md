# GitNuestro-kw
Git nuestro :)

1. Deshacer un commit *perdiendo los cambios en el Working Copy*
>user$ git reset --hard HEAD~1 (Debido a que de este modo perdemos los cambios del Working Copy)

2. Rehacer el último commit *deshaciendo el que acabamos de deshacer*
>user$ git reflog (Nos muestra todos lo commits de nuestro repositorio y en orden desde más nuevo a más antiguo)
>user$ git reset --hard idCommit (volvemos a recuperar el commit perdido)

3. Hacer un merge con ‘master’ *styled absorbe a master*
>No, causa ningun conflicto ya que se ha modificado el archivo de la rama styled. Y la rama master absorbe la cambios realizados en la rama styled.

4. Hacer un merge de “htmlify” en “styled” *styled absorbe a htmlify*
>No, la rama style absorbe el trabajo realizado en la rama htmlify, ya que al estat en la misma lista solo actiza la rama hasta ese punto.

5. Desde “master”, hacer un merge con “styled” *master absorbe a styled*
>No, porque del mismo modo se actuliza la rama al listado correspondiente al que apuntan las ramas.

6. Dibujar el diagrama
>user$ git log --graph --decorate --pretty-oneline
*Para utilizar un solo comando >user$ git log --graph 
>git config alias.graph "log--graph --decorate --pretty-oneline"

7. Hacer un merge “no fast-forward” de “title” en “master” *master absorbe a title*
> Podria ser un merge fast forward y simplemnte desplazar la rama master a ese punto. Al forzar un merge no Fast Forward dejamos constacia de un commmit nuevo en el grafo.

8.  Desacer el merge *Comandos utilizados* (Sin perder los Working Copy)
>  user$ git reset HEAD~1
> user$ git status 

9.  Descartar los cambios 
> user$ git checkout --NameFile 
> user¢ git status

10. Eliminar la rama *title*
>user$ git branch -D title 

11. Rehacer el merge que hemos deshecho
>user$ git reflog
>user$ git reset --hard idCommit 
>user$ git reset --hard ec2635e

12. Volver al commit inicial cuando se creó el poema
>user$ git reset --hard 2f59ed3

13. Volver al estado final, cuando pusimos título al poema
>user$ git reset --hard ec2635e
