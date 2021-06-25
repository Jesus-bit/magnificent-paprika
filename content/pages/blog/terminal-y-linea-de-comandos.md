---
title: Terminal y linea de comandos
date: '2021-06-25'
thumb_image_alt: lorem-ipsum
image_alt: lorem-ipsum
excerpt: Aprende lo Básico de terminal
seo:
  title: ''
  description: ''
  robots: []
  extra: []
  type: stackbit_page_meta
layout: post
image: /images/cli.png
thumb_image: /images/happy-chili.png
---
## ¿que es la terminal?

Es la ventana que aloja una shell. Una shell es una forma de comunicarnos directamente con el sistema operativo.

### ¿por que aprender de terminal?

*   Flexibilidad: es decir puedes hacer tareas con mucha facilidad para diferentes casos

<!---->

*   Velocidad: es muy veloz para hacer procesos que necesites o tareas

*   La interfaz gráfica hace que los procesos sean mas lentos

### Tipos de lineas de comandos

Las mas populares son:

*   Bourne Shell

*   Bash Shell (Es la mas común)

*   Z Shell

*   C Shell

*   Korn Shell

*   Fish Shell

# ¿Qué es un comando?

**Un comando puede ser 4 cosas:**

*   Un programa ejecutable: que se compilo en algun lenguaje de programación y se puede ejecutar

*   Un comando de utilidad de la shell.

*   Una función de shell

*   Un alias

**Comandos**

*   **type** nos permite saber que clase es un comando. Por ejemplo type cd (es una funcion de shell), ls (es un alias)

<!---->

*   Con **–help o help**, puedes tener una ayuda sobre los comandos.

*   **man ‘comando’** : hace referencia al manual de usuario de un comando, otro similar es informático

*   **whatis ‘comando’** : nos da una descripcion muy corta de que hace ese comando. Pero no funciona con todos.

### Comandos Basicos de la terminal

\*\*Mostrar información del directorio: \*\*

**ls** :Lista el contenido de los directorios (por defecto ordena la salida alfabéticamente).

**Alguna de sus opciones (argumentos) más útiles son:**

*   **a** :todos los archivos, incluso los que comienzan con punto (.).

*   **A** :Lista todos los ficheros en los directorios, excepto los que comienzan con punto . (.) y los que comienzan con doble punto (…).

*   **F** :indica tipo: / directorio, \* ejecutable, @ enlace simbólico.

*   **h** :indicará el tamaño en KB, MB, etc.

*   **l** :listado en formato largo (o detallado).

*   **S** :clasifica los contenidos de los directorios por tamaños, con los ficheros más grandes en primer lugar.

*   **r** :invierte el orden de la salida.

*   **R** :Lista recursivamente los subdirectorios encontrados.

*   **t** :ordenar por fecha de última modificación.

*   **u** :ordenar por fecha de último acceso.

*   **x** :presenta los ficheros por columnas.

*   **i** :precede la salida con el número de i-node

Identificar la ruta en la que estamos en nuestro sistema: > pwd

Movernos entre directorios:  > cd

Crear un directorio: > mkdir

Copiar un archivo:  > cp

Borrar un archivo:  > rm

Mover un archivo:   > mv

Borrar un directorio:  > rmdir

Limpiar la terminal:  > clear

Atajo para limpiar pantalla

**ctrl + l**

# Wildcards

Las wildcards nos sirven para realizar seleccionamiento de archivos o directorios, ademas de "ls" los wildcards también pueden usarse con cualquier comando que realice la manipulación de archivos como mv, cp y rm. Ejemplo:

*   \>ls \*.txt //todos los *archivos* con *extensión* txt se mostraran

*   \> ls archivo\* //mostrara todos los que tengan al inicio del nombre "archivo" independiente de la extensión o caracteres que tenga

*   \> ls archivo? //mostrara todos los archivos que tengan el nombre "archivo" al inicio y al final tengan cualquier otro carácter pero solo uno

Entonces en resumen, el "  \*  " se expande de 0 a más caracteres, mientras que "?" expande a uno exactamente.

## Redirecciones I/O y operadores de control:

*   comando < archivo      Redirige el input de un comando hacia un
    archivo

<!---->

*   comando > archivo  -Redirige la salida de un comando a un
    archivo (usarse con cuidado porque
    sobrescribe el sistema)

*   comando >> archivo  -Concatena la salida de un comando a un
    archivo. Si no existe lo crea.

*   comando 2> error.txt -Redirige la salida de error de un comando
    al archivo error.txt

*   comando1 | comando2 -Redirige la salida del comando1 a la
    entrada del comando2

*   comando1; comando2  -Ejecuta de manera consecutiva

*   comando1 & comando2  -Ejecuta de manera asíncrona

*   comando1 && comando2  -Ejecuta el comando2 si y solo si el
    comando1 se ejecutó de manera exitosa

*   comando1 || comando2  -Ejecuta el comando1 o el comando2

# Cómo se manejan los permisos

permisos de:

*   r = read = lectura = 4

*   w= write = escritura = 2

*   x = executable = ejecutable = 1

Para cambiar los permisos se utiliza el comando chown (Change Owner) y luego un numero el numero que le des como parámetro dependerá de que permisos le quieres dar al archivo para saber que numero debe ser solo tienes que sumar los numero que tienen en octal cada permiso por ejemplo: ´chown archivo.txt 555´ el 5 es de lectura y ejecutable y se coloca tres veces por que cada una pertenece a un grupo, lo grupos que existen son:

*   usuario

*   grupo

*   otros(world = mundo)

El usuario es el dueño del archivo o quien lo creo. El grupo son los miembros de un grupo de usuarios. Otros son los usuarios que no están ni en en el grupo ni son propietarios.

## Alias en la terminal

Los comandos alias de la terminal nos permiten crear comandos personalizados con nombres más cortos o fáciles de recordar. De esta manera, estos comandos alias pueden llamar comandos más complejos e incluso otros comandos alias. Estos alias son temporales y solo viven cuando la sesión en que hiciste el alias sigue viva.

Para crear un alias: 

**alias ‘nombreDelAlias’** = **‘comandoQueInvoca’**.

Por ejemplo: alias l=”ls -lh”.

# Variables de entorno

Las variables de entorno son valores dinámicos que afectan los procesos o se utilizan para el flujo de trabajo de la terminal. Existen en todos los sistemas operativos y su tipo puede variar. Las variables de entorno se pueden crear, editar, guardar y eliminar.

*   env -Imprime las variables de entorno actuales

*   echo $VAR -Imprime la variable de entorno VAR

*   $PATH  -Variable donde están las rutas de los
    ejecutables

podrias crear varibles de entorno modificando el archivo .bashrc o .zshrc depende que tipo de terminal tengas para saber como se llama el archivo que tienes que modificar. puedes abrir este archivo colocandote en el dirtectorio raiz de tu usuario normal (no el superusuario) usando el editor de terminal nano lo abres:

\>nano .bashrc

Y agregas una nueva linea que diga:

\`

alias Nombredelalias = 'comandoEquivalente'

\`

# Comandos de búsqueda

which : este comando va a buscar los programas que tengas instalados en la variable de entorno PATH

find: ARGUMENTOS

*   \-type (d = directorios, f = archivo,)

*   \-size (en MB GB B KB)

El comando whereis (en español: ¿dónde está?), este comando es algo similar a which, pero mucho mejor. Este comando localiza los ficheros binarios, fuentes y páginas del manual de un programa, es decir, podemos decir que hace algo así como una “búsqueda mucho más profunda”, me encanta porque puedes saberlo casi todo sobre la ubicación de un programa.

# Grep

podriamos hablar de grep en un post entero pero te dare la introducciongrep es un comando con muchas utilidades, la verdad es que tiene muchos casos de uso, aquí te dejo algunos que a mí me han sido de utilidad 👀👇:

