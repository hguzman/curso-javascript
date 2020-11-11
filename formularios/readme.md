# Formularios
En realidad un formulario es una tematica relacionada con HTML, pero en esta sección trabajaremos en como interactuar entre un formulario y javaScript

```javaScript
function holaMundo(){
  alert("Hola mundo");
}
```

```html
<form>
  <input type="button" value="Click por favor" onClick="holaMundo()">
</form>
```

## Controles de formulario

### Tipo text

```html
<form>
  <input type="text" name="" value="" id="nombre">
  <input type="button" value="Click por favor">
</form>
```

```javaScript
var nom = document.getElementById('nombre').value;
```

## Controles de formulario

### Tipo select

```html
<form name="formulario">
  <select name="desplegable">
    <option value="10">Bueno</option>
    <option value="5" selected>regular</option>
    <option value="0">Malo</option>
  </select>
  <input type="button" value="Click por favor">
</form>
```

```javaScript
var t = document.formulario.desplegable.length; // Número de opciones
var selecionado = document.formulario.desplegable.selectedIndex; // Indice seleccionado
var sel = document.formulario.desplegable.options[0].text;
```
