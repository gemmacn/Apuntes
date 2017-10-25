GITHUB
======
password:460Tomo:

####Como clonar un repositorio de la web en local ( el enlace es el que te proporciona al darle al botón clonar)
 git clone https://github.com/manuelbarzi/skylab-bootcamp-201709.git
-------------------------------------------------------------------------------
Se usan comandos de consola mezclados con los del GIThub

pasos tipicos:
git pull
haces los cambios

( si no quieres que alguno de tus archivos modificados en local tenga conflicto ccon lo s que te estas descargando con el pull, por ejemplo, no quieres tu versión sinó la descargada, haces git checkout -- filename.js, eso hace que este documento se machaque con el pull que t descargas)
git add README.md
git commit -m "nuevos cambios por ejemplo"
git push
git status

origin: esel repo remoto
master: rama principal local o remota
working copy------> a través del add y el commit lo añado a la cajonera. Cda vez se va creando un nuevo HEAD. El HEAD es la ultima versión, tanto en cada rama como en la master.

Cada commit es un punto en la historia de mi repositorio

Cuando hago un push toda la historia y docs de mi local me pasa al remoto ( la web)

Tengo que situarme en la rama donde quiero merchear, a la de destino----------> git merge develop. ( desde la rama maestra mercheame dvelop)
 + git push


git branch -d develop------------> delete develop once it's merged.

git add remote -------------> para subir a la web

git init-bare ----->me ha creado un repositio maestro en mi pc 
git init ------------->me crear un local que no esta conectado con ningun repo maestro remoto.
git clone ----->clonar el repo en local.
git status---------> ver lo que hay dentro de un folder
git add---------> añadir un archivo al control de versiones ( git add README.md ) Aún no esta subido,esta preparado. Se le llama "staging". Aún estamos en local...
git add . ----------> el fichero/ archivo lo añado al control de versiones 

git rm  --cached README.md ---------->lo tiro para atrás en el "staging", al final no quiero subirlo.


git commit -m ----------> ya forma parte de la historia de mi caja / repositorio local. ( mi caja), 
Si después de esto hago un push se me sube a la web



git pull -----------> mi repo local los sincroniza a remoto, si hay archivos nuevos añadidos me los sincroniza en mi repositorio local
git push -------> subir al repo remoto

git checkout + el codigo numerico de la version ---------> me reemplazada con la utima versión que tengo guardada
Para ver la lista de cambios ------------> git log
Pero me crea un nuevo HEAD una nueva linea del archivo. Se usa para consultas pero no es bueno trabajar  sobre el HEAD recuperado pq estoy en otro camino de versiones, digamos..



 puedo poner la direccion de la version que quiero.
git checkout ----> moverte entre ramas
git checkout -b ramanueva ------------> te crea una rama nueva y te mueve a ella. Al crear una rama me copia automático el contenido que habia en la rama Master.


git log ------------> veo que hay en el maestro, veo la lista de cambios y quien los ha hecho





 1. creo una carpeta : mkdir Principal
 2. cd principal
 3. git init--bare
 4. git status
 5. pwd
 

 
#####el head es la ultima version de un fichero 
git HEAD HEAD-----> 
git diff -----> Ver las diferentes versiones


.gitingnore ---------------->   le dices a git que ese directorio no lo tenga en cuenta a la hora de subir una carpeta



En el maestro nunca voy a ver los archivos. 

Para ver cambios de los demás tengo q refrescar el repo maestro y si alguien ha  hech un cambio yo tendré q descargarme la ultima versión antes de poder hacer un push.  Haces un  git pull y te bajas la version que otros han modificado.


Actualizar  un fork:

( Nos bajamos las actualizaciones del dueño original del fork al local, y luego eso actualizado se sube a nuestro fork en remoto. La info hace una V )
=================================
      Desde dentro de la carpeta del fork en local :
     - git remote -v
     - git remote add upstream https://github.com/manuelbarzi/skylab-bootcamp-201709.git ------> la direccion del repo original ( del usuario original, no del mio)
     - git remote -v -----> 
     - git fetch upstream--------------> trae los cambios del remoto a la base de datos local.
       Como ya tienes el upstream a partir de ahora con el fetch se irá actualizando...
       upstream es el repositorio del dueño aoriginal del fork
     - git merge upstream/master ---------------->from upstream(manuelbarzi) master to local master ( branch master)
     - git status
      -git push

      -------------------------------------------

fetch ---trae los cambios a local pero no los ejecuta







git add + git commit -----> lo meto en mi caja definitivament

en la web: settings-- github-- colaborators, para invitar a alguien a tu github

Las carpetas vacias no las muestra al ls 
--------------------------------------------------------------------------
start a working area (see also: git help tutorial)
   clone      Clone a repository into a new directory
   init       Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add        Add file contents to the index
   mv         Move or rename a file, a directory, or a symlink
   reset      Reset current HEAD to the specified state
   rm         Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect     Use binary search to find the commit that introduced a bug
   grep       Print lines matching a pattern
   log        Show commit logs
   show       Show various types of objects
   status     Show the working tree status

grow, mark and tweak your common history
   branch     List, create, or delete branches
   checkout   Switch branches or restore working tree files
   commit     Record changes to the repository
   diff       Show changes between commits, commit and working tree, etc
   merge      Join two or more development histories together
   rebase     Reapply commits on top of another base tip
   tag        Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch      Download objects and refs from another repository
   pull       Fetch from and integrate with another repository or a local branch
   push       Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.


