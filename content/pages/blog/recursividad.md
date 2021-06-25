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
  
  
  **Un ejemplo en codigo (Javascript)**
  `  
    
    function cuentaRegresiva(numero){
      numero = numero - 1 ;

      if(numero > 0);
          console.log(numero);
          cuentaRegresiva(numero);
      else:
          console.log("Feliz año nuevo")

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
      Feliz año nuevo
    }
     
    
    `  


  **Soluciones iterativas**
  
 para resolver el caso anterior de una forma iterativa quedaria como:  
 
 `
    
    function cuentaRegresiva(numero){
    
      for(i = 1; i < numero; i++){
        console.log(numero);
      }
      
      console.log("Feliz año nuevo");
    };
    
 
 `  
 
 **Caso base**  
 
 Como veras para que en la solucion recursiva, no caiga en un loop infinito debe haber un indicador para que se detenga. A esto se le conoce **Caso base**
