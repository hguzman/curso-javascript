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
