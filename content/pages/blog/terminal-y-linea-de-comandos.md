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

*   Para crear un alias: **alias ‘nombreDelAlias’** = **‘comandoQueInvoca’**. Por ejemploalias l=”ls -lh”. Temporales, por el momento.

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

comando < archivo Redirige el input de un comando hacia un
archivo

*   comando > archivo Redirige la salida de un comando a un
    archivo (usarse con cuidado porque
    sobrescribe el sistema)

*   comando >> archivo Concatena la salida de un comando a un
    archivo. Si no existe lo crea.

*   comando 2> error.txt Redirige la salida de error de un comando
    al archivo error.txt

*   comando1 | comando2 Redirige la salida del comando1 a la
    entrada del comando2

*   comando1; comando2 Ejecuta de manera consecutiva

*   comando1 & comando2 Ejecuta de manera asíncrona

*   comando1 && comando2 Ejecuta el comando2 si y solo si el
    comando1 se ejecutó de manera exitosa

*   comando1 || comando2 Ejecuta el comando1 o el comando2
