# Comandos Iniciales :innocent:

Ahora sí veremos cuáles son los comandos principales de **Git** y así comenzar a trabajar con él de manera efectiva:

- **`git init:`** El principal comando pues crea un repositorio vacío dentro del directorio en el cual te encuentres. Cra una carpeta **.git** invisible que puedes ver configurando el Explorador de Archivos u el programa que uses.   
<br> <img src= Images/Comandos%20Iniciales/git_init.png>  
  - Una vez hagas esto el nomrbre del directorio tendrá una etiqueta *MASTER* o *MAIN* que representa que es un repositorio de **Git** funcional.  

  - Esta etiqueta representa que te encuentras en la Rama Principal del proyecto, de dónde saldrán las demás subramas del proyecto.  
  
  - **`git branch -m "NombreRama":`** Este comando permite cambiar el nombre de la rama principal en donde te encuentras.

- **`git status:`** Comando que nos permite ver el estado de las ramas dentro de nuestro proyecto, permite ver también todos los archivos que hay dentro.  
<br><img src = Images/Comandos%20Iniciales/git_status.png>  
  - Nos permite ver también qué archivos han sido modificados para de esta manera tener una visión clara de lo que podrías deseear guardar.  

- **`git add + "Archivo":`** Comando que nos permite añadir un archivo o carpeta a un índice especial, como lo es seleccionar fotos dentro de una galería para poder realizar una acción con ellas.  
<br><img src=Images/Comandos%20Iniciales/git_add.png>
  - Luego de colocar un archivo en el índice podemos volver a usar el comando git status para ver que ese archivo está seleccionado.
  - **`git add .:`** Si colocamos el comando seguido de un punto se seleccionarán todos los archivos del directorio en que te encuentres.
  
- **`git commit:`** Comando que sirve para realizar nuestro primer guardado, es uno de los que más se debe usar y guarda todo lo que hayas añadido a la lista con "add"  
<br><img src=Images/Comandos%20Iniciales/git_commit.png> 
  - Para realizra un commit se debe tener un comentario que nos permita identificar el commit, de otra manera no se permitirá realizar. También puedes añadir una descripción.
  - **`git commit -m "Comentario":`** Permite realizar el commit con un comentario asociado que puedes Modificar.
  - Todos los commits tiene un código único que los permite diferenciarlos de los demás. Se le llama Hash

- **`git log:`** Permite ver los commits realizados, mostrando el usuario que lo realizó, su email, la fecha y hora; además del comentario y descripción asociado al commit.  
<br><img src = "Images/Comandos%20Iniciales/git_log.png">
  - **`git log --graph:`** Permite ver una línea de ramas de nuestro trabajo y así tener un orden de los cambios realizados.

- **`git checkout + "Archivo":`** Sirve para devolver un archivo modificado a un estado inicial, en este caso el estado en que se encontraba luego de hacer el úlitmo commit.

- **`git diff:`** Permite ver los cambios que se han hecho en archivos modificados, desde lo nuevo que has añadido he incluso lo que se ha borrado con el fin de tener esta comparacion que puede resultar util.  
<br><img src = Images/Comandos%20Iniciales/git_diff.png>