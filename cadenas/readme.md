# Manejo de cadenas

En JavaScript las cadenas se manejan con un objeto llamado string, el cual expone algunos atributos y metodos que nos facilitan el trabajo con cadenas de texto.

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
Para concatenar cadenas de texto se puede utilizar el operador **+** como se muestra en el siguiente

:point_right:**EJEMPLO:**

```javascript
var cadena1 = "Aprendiendo a";
var cadena2 = "programar en ";
var cadena3 = "JavaScript";

 var cadena4 = cadena1 + " " + cadena2 + cadena3;

console.log(cadena4);  // Devuelve "Aprendiendo a programar en JavaScript"
```

Otra forma de hacerlo es utilizando el metodo concat() de la clase String()
  
:point_right:**EJEMPLO:**

```javascript
var cadena1 = "Aprendiendo a ";
var cadena2 = "programar en";
var cadena3 = "JavaScript";

var cadena4 = cadena1.concat( cadena2, " ", cadena3 );

console.log(cadena4);  // Devuelve "Aprendiendo a programar en JavaScript"
```
