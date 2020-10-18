# Funciones

Es un bloque de codigo empaquetado y aislado que realiza una tarea específica, cone el proposito es reutilizar codigo 

```javascript
//definimos la función, que en este caso la llamamos saludo()
 
function saludo() { 
     document.write("Hola, este es el resultado de la función saludo");
}

//llamamos a la función saludo() para que ejecute sus instrucciones
 
saludo();
```

## Funciones con parametros

La funciones tambien permiten recibir parametros (variables) con el fin de alimentar el codigo empaquetado.

```javascript
function suma(num1, num2, num3){
 var suma;
 suma = num1 + num2 + num3;
 document.write("Suma = ", suma);
}

var n1, n2, n3;
n1 = 3;
n2 = 5;
n3 = 2;

suma(n1, n2, n3);
```
