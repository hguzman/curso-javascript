# Clase Math

Esta clase provee los metodos necesarios para realizar operaciones matemáticas complejas. Ej: seno, coseno, potencias

```javascript
var num = new Number(Math.random()*10);
document.write('El número aleatorio es: ', num);
document.write('<br>');
document.write('Su raiz cuadrada es: ', Math.sqrt(num));
```

# Algunas de las clases mas utilizadas son: 

**Math.abs()**: Nos devuelve el valor absoluto de un numero.

**Ejemlo**

let number = -25; 
**Math.abs(number)** nos devolvera 25 


**Math.ceil()** Esta nos devolvera un numero redondeado al mas lejano sin importar que el numero
se encuentre mas cerca de su mismo valor.

**Ejemlo**

let number = 23.3;
**Math.ceil(number)** nos devolvera 24


**Math.floor()** Su funcion es similar a Math.ceil, la gran diferencia es que lo hace a la inversa.

**Ejemlo**

let number = 25.8;
**Math.floor(number)** nos devolvera 25


**Math.pow()** La funcion de pow es elevar el numero a x potencia.

**Ejemlo**

let number1 = 10;
let number2 = 6;

**Math.pow(number1, number2)**; Se podria decir que esta funcion es igual 10 elevado a la 6.


**Math.round()** Esta funcion redondea el numero ya sea mas cercano o mas lejano, dependiendo del decimal.

**Ejemlo**

let number = 10.98868

console.log(Math.round(number)) Se podria decir que el numero mas cercano es 11.




