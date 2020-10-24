# Funciones

Es un bloque de código **empaquetado** y **aislado** que realiza una tarea específica, con el propósito es reutilizar código 

```javascript
//definimos la función, que en este caso la llamamos saludo ()
 
function saludo () { 
     document. write ("Hola, este es el resultado de la función saludo");
}

//llamamos a la función saludo () para que ejecute sus instrucciones
 
Saludo ();
```

## Funciones con parámetros

Las funciones también permiten recibir parámetros (variables) con el fin de alimentar el código empaquetado.

```javascript
function suma (num1, num2, num3) {
 var suma;
 suma = num1 + num2 + num3;
 document. write ("Suma = ", suma);
}

var n1, n2, n3;
n1 = 3;
n2 = 5;
n3 = 2;

suma (n1, n2, n3);
```

:key: **EJERCICIO: **
Hacer un programa que utilice una función para realizar operaciones matemáticas básicas, la función debe recibir 3 parámetros como se describe a continuación
* Parámetro 1: Un número que indica la operación que se realizara (1 = Suma, 2 = resta, 3 = Multiplicación, 4 = división)
* Parámetro 2: Primer número objeto de la operación matemática
* Parámetro 3: Segundo número objeto de la operación matemática


## Funciones que devuelven valores

Una de las características más importantes de una función es que pueda devolver un valor, esta característica permite mantener independencia del programa principal.

```javascript
function suma (num1, num2) {
  var n = num1 + num2;
  return n;
}

var resultado = suma (3, 5);

document. write ('La suma es: ', resultado);
```


## Funciones flecha (Arrow functions)

Las arrow functions es una nueva forma que trae Javascript para escribir funciones, para explicar su sintaxis usaré el mismo ejemplo que se usó en la parte de **Funciones que devuelven valores**

```javascript
const suma = () => {
  let n = num1 + num2;
  return n;
}

let resultado = suma (3, 5);

document. write ('La suma es: ', resultado);
```

Como se ve en el ejemplo anterior la palabra **function** fue remplazada por una flecha (=>) por eso el nombre de funciones flecha.
