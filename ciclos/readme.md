# Ciclos

Un ciclo es una estructura de programación que permite repetir un bloque de instrucciones.

Los ciclos mas utilizados son:

# Ciclo mientras que (While)

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

**IMPORTANTE:**  Es muy común cuando se esta empezando, cometer un error en este tipo de bucles. Los bucles While SIEMPRE tienen que modificar los valores de la condición...En este caso, la "n", dentro del bucle se tiene que modificar...porque si no nunca va a ser falsa la condición, y por tanto se producirá un bucle infinito.
