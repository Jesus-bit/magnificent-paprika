---
title: Como configurar llaves ssh para git y github
subtitle: Lo mejor es llaves ssh a usuario y contraseña en HTTPS
date: '2021-06-27'
image_alt: conexión de git a github
excerpt: Como configurar conexión con github
seo:
  title: ''
  description: ''
  robots: []
  extra: []
  type: stackbit_page_meta
layout: post
thumb_image: >-
  /images/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f323733322f312a6d74736b3366515f4252656d466964686b656c3364412e706e67.png
image: >-
  /images/68747470733a2f2f6d69726f2e6d656469756d2e636f6d2f6d61782f323733322f312a6d74736b3366515f4252656d466964686b656c3364412e706e67.png
thumb_image_alt: 'conectar de git a github '
---
# Configuara llaves ssh de git y github

## ¿por que es usar llaves ssh?

cuando tu utilizas github desde la web es seguro el protocolo HTTPS pero tiene un problema por que para accesader a tu github utilizas usuario y contraseña pero ese usuario y contraseña se guardan de forma local ,es decier, en tu computadora y si por alguna razon te llagan a robar la computadora, el atacante pueden tener acceso a los proyectos de tus cliente o al proyecto de empresa para que trabajas.

**Generar una nueva llave SSH: (Cualquier sistema operativo)**

ssh-keygen -t rsa -b 4096 -C "youremail@example.com"

**Comprobar proceso y agregarlo (Windows)**

*   eval $(ssh-agent - s)

*   ssh-add ~/.ssh/id_rsa

**Comprobar proceso y agregarlo (Mac)**

*   eval "$(ssh-agent -s)"

*¿Usas macOS Sierra 10.12.2 o superior?*
*Haz lo siguiente:*

*   cd ~/.ssh

*   Crea un archivo "config…"

*   Con Vim "vim config"

*   Con VSCode "code config"

*   Pega la siguiente configuración en el archivo…

Agrega tu llave

ssh-add -K ~/.ssh/id_rsa
🥳
