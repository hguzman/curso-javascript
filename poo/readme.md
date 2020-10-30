# POO (Programación Orientada a objetos)

La idea de la programación orientada a objetos es que el programador visione la problemática como en la vida real.

El elemento básico de este paradigma no es la función (elemento básico de la programación estructurada), sino un ente denominado objeto.

**NOTA:**
Desde aquí pensaremos en clases y objetos.

## Clases
Una clase es una estructura necesaria para crear los diferentes objetos

![clase carro](https://aprendiendoarduino.files.wordpress.com/2017/07/clase_coche.png)

![clase persona](https://www.campusmvp.es/recursos/image.axd?picture=/2019/4T/poo-clase-objetos.png)

![clase homero](https://ferestrepoca.github.io/paradigmas-de-programacion/poo/poo_teoria/images/philosophy.png)

## Clase Date
Javascript como lenguaje de programación implementa el paradigma Orientado a Objetos, por lo cual ya tiene algunas clases definidas por defecto.

La clase Date por ejemplo tiene la estructura necesaria para construir objetos que permiten hacer operaciones con fechas.

```javascript
var fecha = new Date();
fecha.getFullYear();
// Muestra el año actual
```

**NOTA:**
>De debe tener en cuenta la notación punto para accedes a los atributos y metodos

### Metodos

* `getFullYear()`Año (actual)
* `getHours()`Horas (actual)
* `getMinutes()` Minutos (actual)
* `getSeconds()`Segundos (actual)

### Reto

![ejemplo fecha](img/fecha.png)

## Clase Array
Es una estructura de programación que permite implementar un vector.

```javascript
var vector = new Array(3);
vector[0] = 3;
vector[1] = 1;
vector[2] = 7;
document.write(vector[0],'<br>');
document.write(vector[1],'<br>');
document.write(vector[2],'<br>');
document.write('La longitud del array es: ', vector.length);
```

**NOTA:**
>Cuando los array tienen muchos elementos se debe utilizar un ciclo, uno de los ciclos mas utilizados para este proposito es el _para_.

## Clase Math
Esta clase provee los metodos necesarios para realizar operaciones matemáticas complejas. Ej: seno, coseno, potencias

```javascript
var num = new Number(Math.random()*10);
document.write('El número aleatorio es: ', num);
document.write('<br>');
document.write('Su raiz cuadrada es: ', Math.sqrt(num));
```
