# Selectores

El uso de «selectores» en JavaScript permite encontrar y seleccionar elementos del DOM bien sea para extraer información de cada nodo o para manipularlos de ser necesario.

Estos selectores funcionan de forma  muy similar a los selectores que se usan en CSS.

Metodos utilizados para obtener objetos del DOM
- querySelector
- querySelectorAll

## Selectores mas usados

- `E#myId` un elemento E con ID igual a myID
- `E[foo]` un elemento E con un atributo foo
- `E[foo="bar"]` un elemento E cuyo valor de atributo foo es exactamente igual a bar
- `E[foo~="bar"]` un elemento E cuyo valor de atributo foo es una lista de valores separados por espacios en blanco, uno de los cuales es exactamente igual a bar
- `E[foo^="bar"]` un elemento E cuyo valor de atributo foo comienza exactamente con el string bar
- `E[foo$="bar"]` un elemento E cuyo valor de atributo foo finaliza exactamente el string bar
- `E[foo*="bar"]` un elemento E cuyo valor de atributo foo contiene el substring bar
- `E:visited` un elemento E que es el origen de un hipervínculo cuyo destino ya se ha visitado

## Otros selectores

- getElementsByTagName
- lastElementChild
- getElementsByClassName

## Cambiar propiedades de CSS a través de JS

- `document.querySelector("h1").style.visibility = "hidden";`
- `document.querySelector("h1").classList.add("decorado");`
- `document.getElementsByClassName('someclass').style = "NewclassName";`
- `document.getElementById(id).style.property = 'new style'`
- `document.getElementsByTagName("li");`
- `pic = document.getElementById("Geosam");`
- `pic.src = "sam.jpg";`
