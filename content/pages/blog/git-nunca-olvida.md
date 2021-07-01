---
title: Git nunca olvida
subtitle: git reset y reflog
date: '2021-07-01'
thumb_image_alt: lorem-ipsum
image_alt: lorem-ipsum
excerpt: lorem-ipsum
seo:
  title: ''
  description: ''
  robots: []
  extra: []
  type: stackbit_page_meta
layout: post
---
Git guarda todos los cambios aunque decidas borrarlos, al borrar un cambio lo que estás haciendo sólo es actualizar la punta del branch, para gestionar éstas puntas existe un mecanismo llamado registros de referencia o reflogs.

La gestión de estos cambios es mediante los hash’es de referencia (o ref) que son apuntadores a los commits.

Los recoges registran cuándo se actualizaron las referencias de Git en el repositorio local (sólo en el local), por lo que si deseas ver cómo has modificado la historia puedes utilizar el comando:

Muchos comandos de Git aceptan un parámetro para especificar una referencia o “ref”, que es un puntero a una confirmación sobre todo los comandos:

*   *git checkout  #Puedes moverte sin realizar ningún cambio al commit exacto de la ref = "git checkout eff544f"*

<!---->

*   git reset --hard eff544f *# Perderá todo lo que se encuentra en staging y en el Working directory y se moverá el head al commit eff544f
    *

*   *git reset --soft eff544f # Te recuperará todos los cambios que tengas diferentes al commit eff544f, los agregará al staging area y moverá el head al commit eff544f*

<!---->

*   *git checkout master
    *

*   *git merge eff544f # Fusionará en un nuevo commit la historia de master con el momento específico en el que vive eff544f*
