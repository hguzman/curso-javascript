# Acumuladores

Un acumulador es una variable de incremento o decremento, con valores **inconstantes** durante la ejecución de un programa informático

```javascript
var n = 1;
var suma = 0;
var num;
while (n <= 3){
  num = prompt('Instroduzca número:', '');
  num = parseInt(num);
  suma = suma + num;
  n = n + 1;
}
document.write("La suma de todos los numeros es: " + suma);
```
Además una forma de abreviarlo seria: 

```javascript
var n = 1;
var suma = 0;
var num;
while (n <= 3){
  num = prompt('Instroduzca número:', '');
  num = parseInt(num);
  suma = suma + num;
  n += 1; // "n" es igual a "n+1"
}
document.write("La suma de todos los numeros es: " + suma);
```
 El fragmento de codigo es el mismo, la unica diferencia es la linea 27, que ahora es "n+=1" Esto se traduce en que "n" será igual a "n+1"
