# Ciclos

Un ciclo es una estructura de programación que permite repetir un bloque de instrucciones.

Los ciclos mas utilizados son:

## Ciclo mientras que (While)

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

> **IMPORTANTE:**  Es muy común cuando se esta empezando, cometer un error en este tipo de bucles. Los bucles While SIEMPRE tienen que modificar los valores de la condición...En este caso, la "n", dentro del bucle se tiene que modificar...porque si no nunca va a ser falsa la condición, y por tanto se producirá un bucle infinito.

## Ciclo haga hasta (do/while)

Es un ciclo muy poco usado, lo interesante es qué al menos se ejecuta una vez el bloque de código que se encuentra dentro de la estructura.

Es un comportamiento que no realiza el ciclo mientras que (While)

```
var num = 1;
do{
  document.write(num + "<br>");
  num = num + 1;
}while (num <= 9);
```

**IMPORTANTE:** Tener en cuenta que el hilo de ejecución para comprender que la primera vez siempre ejecutara las instrucciones que estan en el interior del bloque.
