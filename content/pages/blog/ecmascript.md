---
title: ECMAScript 6 +
subtitle: Ecmascript es el estándar de Javascript.
date: '2021-08-11'
thumb_image_alt: lorem-ipsum
image_alt: lorem-ipsum
excerpt: El estándar en javascript
seo:
  title: ''
  description: ''
  robots: []
  extra: []
  type: stackbit_page_meta
layout: post
thumb_image: /images/1da09a35-1e5c-4aef-9317-e88f2cb445d1.png
image: /images/1da09a35-1e5c-4aef-9317-e88f2cb445d1.png
---
## ¿Que es ECMAScript?

**ECMAScript** es la especificación del lenguaje propuestro por **ECMA** Internacional que es una institucíon encargada de los estándares, y JavaScript es el lenguaje de programación que utiliza esta especificación para trabajar sobre estas características que van siendo añadidas año con año desde el 2015.

Cada junio de cada año, y esto es mediante una propuesta, y un comité encargado de revisar estas características que se añadirán al lenguaje.

Lo mas relevante desde el ECMAScript 6 es:

## Arrow Functions y Promesas

**Arrow Functions:  =>**


  `

        const helloPromise = () => {
          return new Promise((resolve, reject)=>{
          if(false){
            resolve('Hello!');
          } else{
            reject('Woops!!');
          }
          });
        }

        helloPromise()
          .then(response => console.log(response))
          .catch(error => console.log(error));

  
`
## Clases y Módulos


`

        // Clases
        class calculator {
          constructor() {
            this.valueA = 0;
            this.valueB = 0;
          }
          sum(valueA, valueB) {
            this.valueA = valueA;
            this.valueB = valueB;
            return this.valueA + this.valueB;
          }
        }

        const calc = new calculator();
        console.log(calc.sum(4, 2)); //6

                // Import
        //Podemos importar solo lo que vamos a utilizar así:

        import { hello } from'./module'

        console.log(hello());
        //También podemos importar más de un elemento separando con una coma

        import { hello, bye } from'./module'

        console.log(hello())
        console.log(bye)

        //Podemos cambiarles los nombres
        import { hello, bye as byeGreeting } from'./module'

        console.log(hello())
        console.log(byeGreeting)
        //Y podemos importar todas las funciones que haya en el archivo

        import * as allGreetings from'./module'

        console.log(allGreetings.hello())
        console.log(allGreetings.bye);


`
## include()

El método **includes()** determina si un array incluye un determinado elemento y devuelve true o false dependiendo si se encuentra o no.

`
        // Antes se utilizaba indexOf para valiar si existia el valor

        let numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9];
        if(numbers.includes(0)){
            console.log('Si está el número.');
        } else{
            console.log('No está el número.');
        }

`
## Object entries

## Spread Operator

## Promise Finally

## Trim

## From Entries

### TC39

EL TC39 es el comité que se encarga de recibir y evaluar las propuestas para agregar a el estándar ECMAScript su pagina oficial es [ESTA](https://tc39.es/)
