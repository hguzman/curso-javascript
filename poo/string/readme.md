# Clase String

En JavaScript las cadenas de caracteres se manejan con un objeto de la clase String, el cual expone algunos atributos y metodos que nos facilitan el trabajo con cadenas de texto, a continuación algunos apuntes importantes.

* [Instanciar un objeto string](#Instanciar-un-objeto-String)
* [Convertir mayúsculas y minúscula](#convertir-may%C3%BAsculas-y-min%C3%BAsculas)
* [Longitud de una cadena](#Longitud-de-una-cadena)
* [Concatenar cadenas](#Concatenar-cadenas)
* [Convertir a cadena de caracteres](#Convertir-a-cadena-de-caracteres)
* [Extraer un caracter](#Extraer-un-caracter)
* [Buscar en una cadena](#buscar-en-una-cadena)


## Instanciar un objeto String
Podemos instanciar un objeto de la clase String y evidenciar su estructura, atributos y metodos.

```javascript
var objCadena = new String("Aprendiendo a programar en javaScript");
console.log(objCadena);
```

:key:**IMPORTANTE:**
>La cadena carga en una estructura tipo **Array** y el primer caracter tiene la posición 0 (cero)


## Convertir mayúsculas y minúsculas
Para realizar este tipo de conversiones, se utilizan los metodos `toLowerCase()` y `toUpperCase() `

:point_right:**EJEMPLO:**

```javascript
var cadena1 = "Aprendiendo a programar en javaScript";

cadena2 = cadena1.toLowerCase();
document.write( cadena2 + "<br />" );  // Devuelve "aprendiendo a programar en javascript"

cadena3 = cadena1.toUpperCase();
document.write( cadena3 + "<br />" );  // Devuelve "APRENDIENDO A PROGRAMAR EN JAVASCRIPT"
```
## Longitud de una cadena
Con la propiedad length obtendremos la longitud de una cadena (espacios incluidos) en JavaScript

:point_right:**EJEMPLO:**

```javascript
var cadena = "Aprendiendo a programar en javaScript";
console.log(cadena.length);  // Devuelve 37
```

## Concatenar cadenas
Para concatenar cadenas de texto se puede utilizar el operador `+` como se muestra en el siguiente

:point_right:**EJEMPLO:**

```javascript
var cadena1 = "Aprendiendo a";
var cadena2 = "programar en ";
var cadena3 = "JavaScript";

 var cadena4 = cadena1 + " " + cadena2 + cadena3;

console.log(cadena4);  // Devuelve "Aprendiendo a programar en JavaScript"
```

Otra forma de hacerlo es utilizando el metodo **concat()** de la clase **String()**

:point_right:**EJEMPLO:**

```javascript
var cadena1 = "Aprendiendo a ";
var cadena2 = "programar en";
var cadena3 = "JavaScript";

var cadena4 = cadena1.concat( cadena2, " ", cadena3 );

console.log(cadena4);  // Devuelve "Aprendiendo a programar en JavaScript"
```
## Otra manera de concatenar es con los template o plantillas.

:point_right:**EJEMPLO:**

let nombre = "David";
let apellido = "Gomez";

console.log(`Hola mi nombre completo es: ${nombre} ${apellido}`);


## Convertir a cadena de caracteres
Podemos convertir un número a cadena concatenando un número con una cadena usando el operador `+`, o bien con la función String() (**no el Objeto del mismo nombre**)

:point_right:**EJEMPLO:**

```javascript
var s1 = "C/Redonda nº " + 3;
var s2 = String(33);
var s3 = String("44 55");
var s4 = String(true);
var s5 = String(false);
var s6 = String( new Date() );
var s7 = String("10/05/2011");

document.write( s1 + "<br />" );   // Devuelve: "C/Redonda nº 3"
document.write( s2 + "<br />" );   // Devuelve: "33"
document.write( s3 + "<br />" );   // Devuelve: "44 55"
document.write( s4 + "<br />" );   // Devuelve: "true"
document.write( s5 + "<br />" );   // Devuelve: "false"
document.write( s6 + "<br />" );   // Devuelve: "Tue May 17 14:41:53 UTC+0100 2011"
document.write( s7 + "<br />" );   // Devuelve: "10/05/2011"
```

## Extraer un caracter
Para extraer un caracter de una cadena utilizaremos el  método charAt() de la clase String, acompañado de la posición dentro del Array de caracteres

:point_right:**EJEMPLO:**

```javascript
var cadena = "Aprendiendo a programar en javaScript";

document.write( cadena.charAt(0) + "<br />" );  // Devuelve 'A'
document.write( cadena.charAt(2) + "<br />" );  // Devuelve 'r'
```

## Buscar en una cadena
En ocasiones necesitaremos averiguar si una cadena de texto en JavaScript contiene a su vez un determinado texto. En tales casos haremos uso del método **indexOf()**, que realizará la búsqueda distinguiendo entre mayúsculas y minúsculas.
Se devolverá la posición en la comienza el texto buscado en la cadena, o bien -1 en caso de que no se encuentre el texto buscado

:point_right:**EJEMPLO:**

```javascript
var cadena = "Aprendiendo a programar en JavaScript";

document.write( cadena.indexOf("JAVASCRIPT") + "<br />" );  // Devuelve -1
document.write( cadena.indexOf("JavaScript") + "<br />" );  // Devuelve 27
```

Podemos indicar que la búsqueda debe comenzar a partir de una determinada posición, indicándola como segundo parámetro

:point_right:**EJEMPLO:**

```javascript
var cadena = "Aprendiendo a programar en JavaScript";
alert( cadena.indexOf("programar", 23) );  // Devuelve -1
```

En este caso se devuelve -1 porque aunque la palabra 'programar' se encuentra en la cadena de texto, la búsqueda comienza después de ella.
También disponemos del método **lastIndexOf()**, que devolverá la posición de la última ocurrencia de una cadena dentro de otra, o -1 en caso de que el texto a buscar no se encontrase

```javascript
var cadena = "Curso de JavaScript: aprendiendo a programar en JavaScript";
alert( cadena.lastIndexOf("JavaScript") );  // Devuelve 48
```

Como vemos, se devuelve la posición 48 aunque la palabra 'JavaScript' se encuentra también en la posición 9 anterior.
Por último, podemos usar también el método **search()**, que al igual que **indexOf()** diferencia entre mayúsculas y minúsculas y devuelve la posición en que se halle el texto dentro de la cadena de texto, o bien -1 si no se ha encontrado

```javascript
var cadena = "Aprendiendo a programar en JavaScript";
alert( cadena.search("JavaScript") );  // Devuelve 27
```

:key:**IMPORTANTE:**
>El método **search()** es usado principalmente con expresiones regulares.

**RETO:**
Una función llamada "letra", que reciba 2 parámetros, una cadena de caracteres, y un índice. La función devolverá la letra cuyo índice ocupe en la cadena. Por ejemplo, si tengo la cadena "Hola", y llamo a la función, le paso la cadena "Hola" y de índice el número 1, el programa devolverá una "o"...O sea, la letra que ocupa la posición del índice en la cadena.
Se debe utilizar un formulario
