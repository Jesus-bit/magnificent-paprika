---
title: Recursividad
subtitle: 'funciones dentro de funciones '
excerpt: >-
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
  incididunt ut labore et dolore magna aliqua.
date: '2021-06-22'
thumb_image: images/13_thumb.jpg
thumb_image_alt: Library shelves
image: https://ichi.pro/assets/images/max/724/1*g8oytHkTTwC68ucOIvlV9A.gif
image_alt: Library shelves
seo:
  title: Recursividad
  description: >-
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
    tempor incididunt ut labore
  extra:
    - name: 'og:type'
      value: article
      keyName: property
    - name: 'og:title'
      value: The function of design is letting design function
      keyName: property
    - name: 'og:description'
      value: >-
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore
      keyName: property
    - name: 'og:image'
      value: images/13.jpg
      keyName: property
      relativeUrl: true
    - name: 'twitter:card'
      value: summary_large_image
    - name: 'twitter:title'
      value: The function of design is letting design function
    - name: 'twitter:description'
      value: >-
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
        tempor incididunt ut labore
    - name: 'twitter:image'
      value: images/13.jpg
      relativeUrl: true
layout: post
---

  **¿Qué es recursividad?** 
  Son funciones que se llaman a sí mismas en el momento que se están ejecutando, es muy importante que tengas en cuenta que las debemos controlar para que no   caiga en un loop infinito y no rompan el flujo normal de nuestra aplicación, debemos tener mucha precaución.
  Lo mejor es condicionarlas y usarlas sabiamente, para que solo se llamen a sí misma bajo una condición que tenga un fin y que luego de ese fin el flujo de la aplicación pueda continuar normalmente. Un gif que lo podra explicar mas graficamente es el de la portada.
  **Un ejemplo en codigo (Python)**
  `def cuentaRegresiva(numero):
    numero = numero - 1 

    if(numero > 0):
        print(numero)
        cuentaRegresiva(numero)
    else:
        print("Feliz año nuevo")

    cuentaRegresiva(10)
9
8
7
6
5
4
3
2
1
Feliz año nuevo`

