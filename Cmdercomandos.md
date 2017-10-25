

![alt text](http://www.skylabcoders.com/images/403/default.png)

 SkyLab BootCamp sep/17
======================

# heading 1
## heding 2
### heding 3
[google](http://wwww.google.es "Google!")

###References in MD
Esto es  [un ejemplo][id]  de link que puedo reutilizar
[id]: http://www.google.es "Titulo opcional del Link"

### Console:
Emulators:
[comader](http://cmder.net)
[cygwin](http://cygwin.com)


### comandos cmder:

Como ver el camino a un directorio de trabajo
Bash es un standard de UNiX, para saber donde stoy
```bash
$ pwd 
```
pwd----------> print working directory
How to list files in directory:
```bash
$ ls
```

Open file:
```bash
$ ls -1a
$ cd folder\
$ cd ..
```


###Bash es el lenguaje que usamos para escribir en la consola. Las instrucciones son para el sistema operativo.

cd.. -----> me lleva a la carpeta padre. Me sube un nivel
. ----> mi carpeta ( donde estoy)
.. ----------> la carpeta padre

cd BootCamp -----> me entra en la carpeta BootCamp 
 cd = change directory ( puedo ir a cualquier carpeta)

rm ------> rm gem.txt  para borrar un solo archivo
rm -r ---------> para borrar un directorio rm -r "carpeta1" y todos sus hijos.
rm -rf w* -----------> borrame las que empiezan por w
rm -d -------->directorio vacio

mover a la carpeta padre un fichero ----> mv README.md ..

mv ----> sirve para mover y cambiar el nombre 
mv folder lav ( me cambia el nombre de folder a Lav)
mv  -r -----------> mv -r file0 file1 -------> mover un fichero con contenido.

crear un fichero ------> touch doc1, touch doc2.....
cp m*.txt file1 ------------> copiame todos los archivos que empiezan por m de la  carpeta donde estoy a la carpeta file1
cp -r dir0/ dir00 ----------> ( directorios)copiame dir0 a dir00. 
cp file0  file1 ----------> (archivos)copiame file0 a file1.

How to create an empty file:
```bash
$ touch <file>
```


Ho to create a directory:

```bash
mkdir <name of directory>
```

Crear un archivo con contenido:
```bash
$ echo "contenido del archivo" > helloworld.txt
```


Ver el contenido de un fichero de texto:
```bash
$ cat <nombrre del fichero>
```

Con less:
```bash
$ less <nombre del archivo>
```


Como linkar una imagen:
```bash
 $ ![alt text](http://www.skylabcoders.com/images/403/default.png)
```


Como crear una Tabla:

```bash
<table>
<tr>
<td>hello</td>
<td>world</td
</tr>
</table>
```

Bloques de codigo:

```bash
<code>
code block
</code>
```


Listados:

```bash
 * hola
 *gemma

 - A
 - B
```

 Podemos usar "<ol> o <ul> / <li> de HTML para hacer listas


 Cursiva y negrita
 ```bash
 *cursiva*
 **negrita**
 ```

 Blockquotes:
 ```bash
 >Quote
 >>nested cuote
 ```

Developer Tools: 

Sources : el codigo que se descarga al navegador 
Network: Monitoriza la comunicación entre el cliente y el servidor y nos permite ver los tiempos de descarga de la info.... 
Performance: Podemos ver cosas que estan en la memoria. Puedo grabar, haceer acciones en las webs y luego me da estadisticas de tiempos etc
Memory: Grabar tmb y me dice lo que ha creado en memoria
Aplication: Cookies y información que se guarda en el servidor, almacenes de datos...








