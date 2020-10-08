# Ciclo haga hasta (do/while)

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
