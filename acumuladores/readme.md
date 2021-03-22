# Acumuladores

Un acumulador es una variable que se incrementa o decrementa con valores variables durante la ejecución del programa. Para ello, lo ideal es incluirlos en bucles. Por ejemplo, crear una variable "acumulador" que vaya sumando 3 números introducidos por teclado. 
 
 
Vamos a ver el código del ejemplo propuesto para entender el uso de acumuladores:

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

lo primero es la creación de variables. 
 
"n" empieza en 1, es la encarga de contar cuantas veces se repetirá el bucle.
 
"suma" es la variable que hace de acumulador, debe empezar en 0.
 
"num" es la variable donde iremos introduciendo los números que pidamos al usuario.
 
 
 
Ahora, comienza el bucle, con la condición de si "n" es mejor o igual que 3 (o sea, el bucle se ejecutará 3 veces, ya que tenemos que introducir 3 números). 
 
Dentro del bucle, pedimos al usuario que introduzca un número y lo guardamos en la variable "num". Convertimos ese número a tipo entero (es muy importante, porque sino el programa trata a esa variable como una cadena de caracteres).
 
Y ahora viene el concepto de acumulador: 
 
suma = suma + num; -> Con esto, vamos añadiendo el valor de "num", al valor que ya tenía "suma" anteriormente, es decir que lo vamos acumulando. Por ejemplo si ha introducido el número 2, se haría: suma = 0 + 2. 
 
Y si luego introduce un 3...
 
suma = 2 + 3...y así sucesivamente. Se van sumando los valores, acumulando el resultado.
 
Luego se le suma +1 a "n" para que cuando llegue a 3, ya salga del bucle while.
 
 
 
Y para terminar, al salir de "while", mostramos el valor de suma por pantalla, para comprobar que se ha realizado correctamente.
