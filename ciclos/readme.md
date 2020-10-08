# Ciclos

Un ciclo es una estructura de programación que permite repetir un bloque de instrucciones.

Los ciclos mas utilizados son:

* [Mientras que (While)](#mientras-que-while)
* [Haga hasta (do/while)](#haga-hasta-dowhile)
* [Para (for)](#para-for)

## Mientras que (While)

La estructura de ciclo While es una de las mas documentadas, el proposito de las estructuras ciclicas es repetir instrucciones o fragmentos de código.

La sintaxis para este lenguaje es la siguiente:

```
var n = 1;
while (n <= 10){
  document.write(n);
  document.write('<br>');
  n = n + 1;
}
```

:key: **IMPORTANTE:**
> Es muy común cuando se esta empezando, cometer un error en este tipo de bucles. Los bucles While SIEMPRE tienen que modificar los valores de la condición...En este caso, la "n", dentro del bucle se tiene que modificar...porque si no nunca va a ser falsa la condición, y por tanto se producirá un bucle infinito.

:fire: **RETO:**
> Construir una pagina que solicite al usuario registrar números menores a 10 y debe imprimirlos en la pagina.
La acción de solicitar número terminara cuando el usuario registre un número mayor a 10.


## Haga hasta (do/while)

Lo interesante es qué al menos se ejecuta una vez el bloque de código que se encuentra dentro de la estructura.

Es un comportamiento que no realiza el ciclo mientras que (While)

```
var num = 1;
do{
  document.write(num + "<br>");
  num = num + 1;
}while (num <= 9);
```

> **IMPORTANTE:** Tener en cuenta que el hilo de ejecución para comprender que la primera vez siempre ejecutara las instrucciones que estan en el interior del bloque.

## Para (for)

La característica principal es que en _teoría_ debe recorrerse completamente.

A diferencia de los "while", el for lleva implícito el aumento o decremento de la variable en cuestión, y en el while había que modificar la variable dentro del bucle.

```javascript
var num = 1;
for (num=1; num <= 5; num++){
  document.write(num + "<br>");
}
```

> **IMPORTANTE:**  Es muy común usar este ciclo para recorrer estructuras de datos como los Array.
