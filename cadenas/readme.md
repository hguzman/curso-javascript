# Manejo de cadenas

En JavaScript las cadenas de caracteres se manejan con un objeto de la clase String, el cual expone algunos atributos y metodos que nos facilitan el trabajo con cadenas de texto, a continuación algunos apuntes importantes.

* [Instanciar un objeto string](#Instanciar-un-objeto-String)
* [Convertir mayúsculas y minúscula](#Convertir-mayúsculas-y-minúscula)
* [Longitud de una cadena](#Longitud-de-una-cadena)
* [Concatenar cadenas](#Concatenar-cadenas)
* [Convertir a cadena de caracteres](#Convertir-a-cadena-de-caracteres)


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
