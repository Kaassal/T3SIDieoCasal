# T3SIDiegoCasal
**Resolucion del ejerecicio 4 Sistemas Informaticos**
## Ejercicio 4
**Partiendo de tu direcctorio de inicio, realiza cada uno de los siguientes apartados** 
## A) Haz que tu directorio de trabajo actual sea el directorio padre de tu directorio de inicio
Tenemos de ir desde home/*usuario* hasta el directorio de inicio, para eso usamos: 

    cd/NombreDirectorioInicio

 
> Si no te acuerdas de los normbres de tus directorios puedes usar
> 
>     ls
> 
> Este comando enumera el contenido del directorio que desee, archivos y otros directorios anidados. 
## B) Visualiza la ruta de tu directorio de trabajo actual
Para visualizar la ruta de trabajo actual usamos:

    pwd
<blockquote> pwd son las siglas de *path workig directory* que significa ruta de directorio en funcionamiento</blockquote>

Despues de escribir pwd la terminak nos devolverá esto :

    home/NombreUsuario/NombreDirectorioInicio

## C) Visualiza todos los ficheros que cuelgan de tu direcctorio de inicio
Para visualizar los ficheros que cuelgan de nuestro directorio de inicio simplemente usamos:

    ls

> Podemos usar solo ls porque ya nos hemos movido al  directorio de inicio usando cd si estuvieramos, por ejemplo en nuestro directorio home ls nos enseñaria los directorios que cuelgan de home, entre ellos el directorio de inicio

El resultado de el comando será una lista de todos los directorios que cuelgan del directorio de inicio

## D) Realiza un listado recursivo de tu directorio de inicio
Para visualizar los ficheros que cuelgan del directorio de inicio de forma recursiva usamos:

    ls -R

> Al usar ls-R está funcionando ls en la carpeta base, y luego en todas las carpetas hijas. El comando va a través de cada carpeta *recursivamente* hasta llegar al final del árbol de directorios. En ese momento, vuelve a subir una rama del árbol y hace lo mismo con las subcarpetas, si las hay.  
  
## E) Obten ayuda del comando *passwd*
Para obtener ayuda del comando passwd podemos usar :

    passwd -h 
o

    passwd --help

> La misma formula de *comando* -h o --help suele funcionar para obtener ayuda sobre la mayoría de comandos de la consola de bash, si no funiciona, info *comando* o man -k *comando* suelen ser alternativas comunes.

## F) Obten la fecha y hora del sistema 

Para obtener la fecha y hora de el sistema usamos:

    date

## G) Con un solo comando posicionate en tu directorio de inicio

Para volver al directorio de inicio con un solo comando usamos:

    cd
    
## H) Crea un fichero materias que contenga el nombre de las materias en las que te has matriculado (cada una en una linea)
Para crear un fichero podemos usar touch:

    touch -NombreFichero
Pero ya que vamos a editarlo tambien podemos crearlo con:

    nano 
El comando nano nos lleva a un editor de texto donde podemos escribir lo que necesitemos,
Usando el comando nano no es necesario introducir un nombre para el fichero para guardarlo, pero si decidimos guardarlo debemos darle un nombre 

> Existen otros editores de texto para bash, siendo los mas comunes ,además de nano, vi, vim y pico. Estos suelen venir instaldos con la distro pero existen muchos otros editores que podemos instalar

## I) Con un solo comando crea dos directorios, *grado* e *Iru*
Para crear varios directorios a la vez usamos el comando mkdir e introducimos los nombres de los directorios entre 2 llaves:

    mkdir {grado,Iru}
    
## J) Usando un solo comando, mueve tu fichero materias para que cuelgue de tu directorio grado pero con el nombre asignaturas.

Para mover el fichero materias a el directorio grado y renombrarlo a materias en el proceso usamos:

    mv materias  /home/diego/grado/asignaturas

## K) Visualiza los ficheros/directorios de tu directorio de trabajo actual y responde a la siguiente cuestión: ¿dónde está tu fichero materias?
El fichero materias *tecnicamente* no existe ya que cuando lo movimos al directorio grado le cambiamos el nombre a asignaturas

## L) Posicionate en tu directorio grado

Para posicionarnos en el directorio grado usamos:

    cd grado

## M) Elimina el fichero asignaturas 

Para eliminar el fichero asignaturas usamos:

    rm asignaturas

## N) Sube al directorio de inicio
   
   Para subir al directorio de inicio usamos:

    cd
## O) Con un solo comando elimina los directorios creados en el paso i)
Para borrar varios directorios a la vez usamos:

    rmdir {gradro,Iru}

> Podemos usar rmdir porque los directorios estan vacios, si tuvieran ficheros habría que moverlos o usar alguna de las opciones de el comando como :
> -   **`-f`**: Fuerza el borrado de todos los directorios y sus ficheros.
>-   **`-i`**: Pide confirmación antes de borrar
>-   **`-I`**: Pide confirmacion cuando se eliminan mas de tres ficheros o se elimina recursivamente
>-   **`-r`**: Elimina recursivamente.
>-   **`-d`**: Elimina directorios vacios.
