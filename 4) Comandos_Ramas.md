# Comandos de Ramas :evergreen_tree:

Ahora veremos que conforme vamos avanzando en **Git**, tenemos mas ramas o puntos de guardado que podriamos desear ver o acceder, es por esto que veremos algunos comando para ramas importantes:

- **`git checkout + CodigoCommit:`** Te permite navegar por los distintos commits que hay, no te dejara si no has guardado todos los cambios. Se cambia la etiqueta HEAD al commit al que has viajado, los commits posteriores no se veran con git log, pues se considera que la cabeza del proyecto donde continuaras es la que tiene la etiqueta HEAD.  
<br><img src = Images/Comandos%20Ramas/git_checkout.png>
  - **`git checkout main:`** Te devuelve al commit main o principal, generalmente el utlimo que has guardado. Por lo general esta etiqueta no cambia a menos que uses el siguiente comando.

- **`git reset:`** (Averiguar)
  - **`git reset --hard + CodigoCommit:`** Este comando sirver para ir a un commit deseado y "eliminar" los commits posteriores en caso no desees trabajar con ellos. Es un comando poco usado ademas debe ser usado con cuidado.

- **`git reflog:`** Sirve para ver todos los commits en los que ha estado la etiqueta HEAD, esto indica tambien los desplazamientos que hemos hecho dentro de las ramas , util para visualizar commits que pueden haberse perdido al usar *git reset --hard*.

- **`git tag + NombreTag:`** Sirve para etiquetar commits con un nombre preferido para recordar mejor o ubicarmos mejor dentro de las ramas. Al colocar el comando pondras el tag al commit donde te encuentres.  
<br><img src = Images/Comandos%20Ramas/git_tag.png>
  - **`git checkout tags/NombreTag:`** Se puede usar el comando checkout con los tags que coloquemos, solo es necesario saber los nombres.
 
- **`git branch + NombreRama:`** Git esta diseñado para que puedas trabajar con varias ramas pues es para equipos de trabajo, este comando permite crear una nueva rama en el commit en donde estas y puedes nombrarla como desees.  
<br><img src = Images/Comandos%20Ramas/git_branch.png>
  - **`git branch -d NombreRama:`** Este comando sirve para elimiar una rama por completo. Es recomendable siermpre realizar un merge antes o guardar los cambios en otro sitio; además de usar el comando con cautela. 

- **`git switch + NombreRama:`** Este comando permite viajar a otra rama creada para realizar los cambios ahi, tambien se podria hacer con el git checkout pero no es muy recomendable cuando se trata de ramas.

- **`git merge + NombreRama:`** Este comando sirve para combinar dos ramas y ver los cambios de ambas, este comando crea un commit nuevo dentro de la rama en la que realizaste el comando.  
<br><img src = Images/Comandos%20Ramas/git_merge_rebase.png>
  - Debido a que *git merge* combina dos ramas, puede haber situaciones en las que haya conflictos pues un mismo archivo se modifico en una rama y en otra, para solucionar esto deberas quedarte solo con uno de los dos cambios y realizar un nuevo *git commit*.
  - Si realizas un "merge" dentro de la rama main entonces podras reintegrar toda una rama dentro de la principal.

- **`git rebase:`** Este comando complejo sirve para, de igual manera que el merge, combinar los cambios realizados en dos ramas, la diferencia es que los commits se combinan también con la rama que desees y se muestran como si nunca se hubiera realizado una rama extra.  
<br><img src = Images/Comandos%20Ramas/git_merge_rebase.png>

- **`git stash:`** Este comando sirve para guardar temporalmente y localmente todos los cambios que hemos estado haciendo en una rama; así podríamos cambiar a otra sin problema sin hacer un commit.  
<br><img src = Images/Comandos%20Ramas/git_stash.png>
  - **`git stash list:`** Podemos ver todos los stash que hayamos hecho hasta el momento.
  - **`git stash pop:`** Si venimos de otra rama y nos situamos ahora en la rama en donde hay un stash, usamos este comando para recuperar los cambios realizados anteriormente.
  - **`git stash drop:`** Sirve para eliminar todos los stash que has realizado localmente.