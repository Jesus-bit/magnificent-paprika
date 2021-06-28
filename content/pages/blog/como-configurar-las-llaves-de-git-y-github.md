---
title: Como configurar llaves ssh para git y github
subtitle: Lo mejor es llaves ssh a usuario y contraseña en HTTPS
date: '2021-06-27'
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
# Configuara llaves ssh de git y github

## ¿por que es usar llaves ssh?

cuando tu utilizas github desde la web es seguro el protocolo HTTPS pero tiene un problema por que para accesader a tu github utilizas usuario y contraseña pero ese usuario y contraseña se guardan de forma local ,es decier, en tu computadora y si por alguna razon te llagan a robar la computadora, el atacante pueden tener acceso a los proyectos de tus cliente o al proyecto de empresa para que trabajas.

**Generar una nueva llave SSH: (Cualquier sistema operativo)**

ssh-keygen -t rsa -b 4096 -C "youremail@example.com"

**Comprobar proceso y agregarlo (Windows)**
`
# Encender el "servidor" de llaves SSH de tu computadora:
eval $(ssh-agent -s)

# Añadir tu llave SSH a este "servidor":
ssh-add ruta-donde-guardaste-tu-llave-privada
`

**Comprobar proceso y agregarlo (Mac)**

`# Encender el "servidor" de llaves SSH de tu computadora:
eval "$(ssh-agent -s)"

# Si usas una versión de OSX superior a Mac Sierra (v10.12)
# debes crear o modificar un archivo "config" en la carpeta
# de tu usuario con el siguiente contenido (ten cuidado con
# las mayúsculas):
Host *
        AddKeysToAgent yes
        UseKeychain yes
        IdentityFile ruta-donde-guardaste-tu-llave-privada

# Añadir tu llave SSH al "servidor" de llaves SSH de tu
# computadora (en caso de error puedes ejecutar este
# mismo comando pero sin el argumento -K):
ssh-add -K ruta-donde-guardaste-tu-llave-privada
`
