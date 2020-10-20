# Acumuladores

Es una variable que incremento o decremento con valores **inconstantes** durante la ejecución de un programa informático

```JavaScript
var n = 1;
var suma = 0;
var num;
while (n <= 3){
  num = prompt('Introduzca número:', '');
  num = parseInt(num);
  suma = suma + num;
  n = n + 1;
}
document.write("La suma de todos los números es: " + suma);
```
