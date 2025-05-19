# Comandos Remotos :joystick:

Git esta diseñado parar trabajar de manera local pero sobre todo para trabajar de manera remota y en equipos de varias personas, es por esto que tambien existen comandos para trabajar con este repositorio remoto.

- **`git remote add origin + NombreRepositorio:`** El comando de remote sirve para conectar el repositorio remoto con el local y asi poder trabajar con ambos.  
<br><img src = Images/Comandos%20Remotos/git_remote.png>  

- **`git push -u origin main:`** Este comando sirve para subir todo lo de la rama main dentro de el repositorio remoto. Se debe colocar la primera vez que realizas un "push".  
<br><img src = Images/Comandos%20Remotos/git_pull_push.png>  
  - **`git push:`** El comando normal se puede utilizar con normalidad luego que se haya realizado el primer "push" y tiene la misma funcionalidad de subir todo.

- **`git fetch:`** Este comando sirve para cargar todos los datos de los commits realizados de manera remota de manera local. Unicamente se tendran la visualizacion del historial de cambios para que puedas verlos pero no cambiara nada.  
<br><img src = Images/Comandos%20Remotos/git_fetch.png>  

- **`git pull:`** Este comando sirve para traer los cambios realizados, este si realiza la accion de traer los datos, si hay cambios entonces se debe de realizar una configuracion especial que provoque que el comando actue de cierta manera similar al *git merge*.  
<br><img src = Images/Comandos%20Remotos/git_pull_push.png>  
    - **`git config pull.rebase false:`** Este comando de configuracion hara que el comando "git pull" actue como "merge"

- **`git clone + NombreRepositorio:`** Este comando sirve para clonar un repositorio remoto. No siempre puedes realizarlo pues esto depende de si el repositorio es publico o privado y si las claves ssh te permiten conectarte.  
<br><img src = Images/Comandos%20Remotos/git_clone.png>