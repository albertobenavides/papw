# Programación de aplicaciones para la Web

## Universidad Autónoma de Nuevo León
## Facultad de Ciencias Físico Matemáticas
## Multimedia y Animación Digital

### Alberto Benavides
### Agosto a diciembre 2018


## ¿Qué es HTML?

* HyperText Markup Language 
 	(Lenguaje de marcado de hipertexto)

* Lenguaje de formato de texto (elementos)
	No un lenguaje de programación

## Elementos HMTL

```html
<p>Este es un párrafo.</p>

<!-- Estructura de un elemento con contenido -->
<etiqueta>Contenido</etiqueta>
```
## Elementos anidados

```html
<p>Este párrafo termina en <i>cursiva</i>.</p>


<p>Aquí hay elementos <i>mal </p> anidados. </i>
```

## Elementos vacíos y atributos

```html
<img src="url.jpg">

<etiqueta atributo="valor">

<etiqueta atributo='valor'>

<etiqueta atributo=valor>
```

## Estructura mínima de un documento HTML

```html
<!DOCTYPE html> <!-- Tipo de documento; histórico -->
<html> <!-- Inicio del documento HTML -->
  <head> <!-- Cabecera; parámetros del documento -->
	<meta charset="utf-8"> <!-- Codificación -->
	<title>Título de la página</title>
  </head> 
  <body> <!-- Cuerpo; todo lo mostrado al usuario -->
	<p>Esta es mi primera página web.</p>
  </body>
</html>
```

## Programas recomendados

#### Editor de texto
1. [Visual Studio Code](https://code.visualstudio.com/)
2. [Atom](https://atom.io/)
3. [Notepad++](https://notepad-plus-plus.org/download/v7.5.8.html)
4. [Sublime Text](https://www.sublimetext.com/)

#### Navegador
* [Chrome](https://www.google.com/chrome/)
* [Mozilla](https://www.mozilla.org/es-MX/firefox/new/)
* [Opera](https://www.opera.com/es-419)

## Control de versiones

Sugerencia:
* Usar [Git](https://www.atlassian.com/git/tutorials/what-is-version-control).
* Usar [Sourcetree](https://sourcetree.com/).

## Instalación de Git

Git | :star: Sourcetree
--|--
1. Bajar e instalar [Git](https://gitforwindows.org/)| 1. Bajar e instalar [Sourcetree](https://www.sourcetreeapp.com/)
2. Abrir terminal | 2. Abrir Sourcetree
3. Insertar código  :small_red_triangle_down: | 3. Tools>Options>General

```git
git config --global user.name "Nombre Apellido" 

git config --global user.email usuario@correo.com
```

## Instrucciones esenciales de Git

```git
rem Inicia un repositorio
git init

rem Prepara un directorio
git add <directorio>

rem Crea un commit (instantánea)
git commit -m "Mensaje"

rem Añade la url como remoto
git remote add <nombre> <url>

rem Envía actualizaciones a un remoto
git push <remoto> <rama>
```

## Encabezados y líneas horizontales

```html
<h1>Encabezado 1</h1>

<h2>Encabezado 2</h2>

<h3>Encabezado 3 sobre una línea</h3>

<hr> <!-- hr: Horizontal rule-->

<h4>Encabezado 4 bajo una línea</h4>

<h5>Encabezado 5</h5>

<h6>Encabezado 6</h6>
```


## Párrafos y saltos de línea

```html
<p>Un párrafo.</p>
<p>Otro párrafo.</p><p>Y otro más</p>

<p>Los      espacios    no      importan.</p>

<p>Ni 
los

saltos
de línea.</p>

<p>Aunque, después de esto <br> hay un salto de línea.</p>
```


## Etiqueta `pre`

```html
<p>
	Las rosas son rojas,
	las violetas azules,
	[...]
</p>

<pre>
	Las rosas son rojas,
	las violetas azules,
	[...]
</pre>
```

## Formato de texto

```html
<p>
    Estas palabras están 
    en <b>negritas</b>, 
    <i>cursivas</i>, 
    son <strong>importantes</strong>, 
    tienen <em>énfasis</em>, 
    aparecen <mark>subrayadas</mark>, 
    <small>pequeñas</small>, 
    <del>tachadas</del>, 
    muestran <ins>inserciones</ins> o 
    <sub>subíndices</sub> y 
    <sup>superíndices</sup>.
</p>
```


## [Código](https://websemantics.uk/articles/displaying-code-in-web-pages/) y [expresiones matemáticas](https://www.mathjax.org/)

```html
<code>int i = 0;</code>

<var>F = m &times; a</var>
```

$$\sum_{i=1}\frac{n!}{r!(n-r)!}^{n}{X_i^2}$$


## Hipervínculos

```html
<a href="https://www.google.com/">Google</a>

<!-- Estructura de un hipervínculo -->
<a href="url">Texto del enlace</a>


<a href="url" target="_blank">Abre en nueva pestaña</a>

<h2 id="ancla">Capítulo cualquiera</h2>

<a href="#ancla">Ir al Capítulo cualquiera</a>

```

## Imágenes y carpetas

```html
<img src="../carpeta/imagen.jpg" alt="Texto alternativo">

<p>
  Imagen a la derecha de 50*50 px
  <img src="url" alt="..." 
  style="float:right;width:50px;height:50px;">
</p>

```

## Listas

```html
<!-- disc, circle, square, none -->
<ul style="list-style-type:disc"> <!-- Lista sin orden -->
  <li>Un elemento</li>
  <li>Otro elemento</li>
  <li>Uno más</li>
</ul>


<!-- 1, A, a, I, i -->
<ol type="1" > <!-- Lista ordenada -->
  <li>Primero</li>
  <li>Segundo</li>
  <li>Tercero</li>
</ol>
```

## Tablas

```html
<table> <!-- Inicio tabla -->
  <tr> <!-- Table row; Fila en la tabla -->
    <th>Nombre</th> <!-- Table heading -->
    <th>Apellido</th>
    <th>Edad</th>
  </tr>
  
  <tr>
    <td>Xavier</td> <!-- Table data -->
    <td>López</td>
    <td>83</td>
  </tr>
</table> <!-- Fin tabla -->

```
Recurso: https://www.tablesgenerator.com/html_tables 


## Bloques

```html
<div>
	Bloque de texto en nueva línea.
	<span>Bloque de texto en la misma línea</span>
</div>
```


## Para saber más: [Markdown](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

```md
# Encabezado 1
# Encabezado 2

Párrafo con *cursiva*, **negritas**, ~~tachados~~.

1. Lista
2. Numerada

* Lista
* No ordenada

[Vínculo a Google](www.google.com)

![Imagen](https://fakeimg.pl/150/)

`código`
```

## ¿Qué es CSS?

* **CSS**: **C**ascading **S**tyle **S**heets
* Hojas de estilo en cascada
* Controlan el diseño de un sitio web
* Se pueden replicar a distintos elementos 


## Sintaxis de CSS

```css
selector{
  propiedad: valor;
  otraPropiedad: otroValor;
}
```

```css
body{
  background-color: blue; /* Color de fondo azul */
  font-size: 18px; /* Tamaño de fuente de 18 pixeles */
}

p{
  color: red; /* Color de texto rojo */
  font-family: Arial; /* Texto con fuente Arial */
}
```


## Insertar CSS
1. Archivo externo vinculado por etiqueta `<link>` dentro de `<head>`
2. Etiqueta `<style>` dentro de `<head>`
3. Atributo `style` en elemento HTML


## Insertar CSS. Archivo externo :star:

1. Crear archivo `nombre.css`
2. Establecer reglas de estilo y guardar

```css
body{
  background-color: green;
}
```
3. Añadir etiqueta `<link>` en documento HTML y guardar

```html
<head>
  <link rel="stylesheet" type="text/css" href="nombre.css">
</head>
```

4. Actualizar, `F5`


## Insertar CSS. Etiqueta `<style>`

1. Añadir etiqueta `<style>` con reglas de estilo en documento HTML

```html
<head>
  <style>
    body{
      background-color: green;
    }
  </style>
</head>
```

2. Guardar

3. Actualizar, `F5`


## Insertar CSS. Atributo `style`

1. Añadir atributo `style` al elemento deseado

```html
<body style="background-color: green;">
```

2. Guardar

3. Actualizar, `F5`


## Selectores de etiquetas

* Seleccionan todos los elementos pertenecientes a la etiqueta especificada

```css
body{}

h1{}

p{}

ul{}

li{}

table{}

img{}

[...]
```


## Atributo y selector `id`
* El atributo `id` permite identificar elementos de manera única

```html
<h1 id="principal">Título principal</h1>

<li id="esencial">Elemento esencial</li>
```

* El selector `id` corresponde al `#`

```css
/* Selecciona el elemento con id="principal" */
#principal{
  font-style: italic; /* Texto en cursiva */
}

/* Selecciona el elemento con id="esencial" */
#esencial{
  font-variant: small-caps; /* Pequeñas mayúsculas */
}
```


## Atributo y selector `class`
* El atributo `class` permite agrupar elementos por un nombre

```html
<h1 class="subrayado">Título subrayado</h1>

<p class="subrayado negritas">
  Varias clases separadas por espacios en blanco.
</p>
```

* El selector `class` corresponde al `.`

```css
/* Selecciona todos los elementos con class="subrayado" */
.subrayado{
  text-decoration: underline; /* Texto subrayado */
}

.negritas{
  font-weight: bold; /* Texto en negritas */
}
```


## Agrupar selectores

* Selectores con mismos estilos pueden agruparse mediante `,`

```css
p{
  text-align: center;
}

h1{
  text-align: center;
}

.rojo{
  text-align: center;
}
```

```css
p, h1, .rojo{
  text-align: center;
}
```


## Propiedades CSS para texto (I)

```css
.ejemplo{
  color: red;
  color: #00ff00;
  color: rgb(0,0,255);
  
  font-size: 15px;
  font-size: large;
  font-size: 150%;
  
  font-style: normal;
  font-style: italic;
  font-style: oblique;
}
```


## Propiedades CSS para texto (II)

```css
.ejemplo{
  font-weight: normal;
  font-weight: bold;
  font-weight: 900;
  
  /* https://fonts.google.com/ */
  font-family: "Times New Roman", Times, serif;
  font-family: Arial, Helvetica, sans-serif;
  
  text-align: center;
  text-align: left;
  text-align: right;
  
  font-variant: small-caps;
}
```


## Propiedades CSS para texto (III)

```css
.ejemplo{
  text-decoration: overline;
  text-decoration: line-through;
  text-decoration: underline;
  
  text-transform: uppercase;
  text-transform: lowercase;
  text-transform: capitalize;
  
  /* https://www.w3schools.com/cssref/css_units.asp */
  text-indent: 50px; /* 50 pixeles */
  text-indent: 2em; /* Relativo al tamaño del elemento */
  text-indent: 30%; /* Relativo al tamaño del padre */
}
```


## Valores de colores para CSS

```css
.ejemplo{
  /* https://www.w3schools.com/colors/colors_names.asp */
  background-color: blue;
  
  /* 
  https://www.w3schools.com/cssref/css_colors_legal.asp 
  */
  background-color: #ff0000;
  background-color: rgb(255, 0, 0);
  background-color: rgba(255, 0, 0, 0.3);
  background-color: hsl(120, 100%, 50%);
  background-color: hsla(120, 100%, 50%, 0.3);
}
```


## Jerarquía de estilo (más interno a más externo)
1. Atributo `style`
2. CSS interno o externo (Los elementos más inferiores tienen preferencia sobre los superiores)
3. Estilo predefinido por el navegador

## Modelo de cajas [ * ](https://www.w3schools.com/css/css_boxmodel.asp)

<center><img src="https://mdn.mozillademos.org/files/13647/box-model-standard-small.png" width="640px"></center>


## Modelo de cajas

```css
div {
    width: 300px;
    height: 200px;
    padding: 25px;
    border: 25px solid black;
    margin: 25px;
}
```


## Alineación de elementos

```css
.centrarEnPantalla {
  margin: auto;
  width: 50%; /* Ancho menor a 100%  */
  border: 3px solid black;
  padding: 10px;
}

.centrarTextoEnElemento {
  text-align: center;
  border: 3px solid black;
}
```


## Selectores combinados [ * ](https://www.w3schools.com/css/css_combinators.asp)

```css
div p{} /* Todos los p dentro de div en cualquier nivel */

div > p{} /* Todos los p hijos inmediatos de div */

div + p{} /* El p que siga de un div hermano */

div ~ p{} /* Todos los p hermanos de div */
```


## Menú vertical CSS [ * ](https://www.w3schools.com/css/css_navbar.asp)

```css
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  width: 25%;
  height: 100%;
  position: fixed; /* Para dejarla fija a la izquierda */
  overflow: auto; /* Desborde con desplazamiento */
}

li a {
  display: block; /* Permite dar clic en toda el área */
  text-decoration: none;
}

li a:hover {
  background-color: #555;
  color: white;
}
```


## Menú horizontal CSS

```css
ul {
  list-style-type: none;
  margin: 0;
  padding: 0;
  background-color: #f1f1f1; /* Color a todo el fondo */
  /* Pegada al desplazar: position: sticky; */
  /* Fija arriba */
  position: fixed; 
  top: 0; /* O abajo: bottom: 0 */
  width: 100%;
}

li { float: left;} /* Cada elemento flota a la izquierda */

li a {
  display: block;
  text-align: center;
  padding: 14px 16px;
}
```


## Menú vertical HTML

```html
<ul>
  <li><a href="#home">Inicio</a></li>
  <li><a href="#news">Servicios</a></li>
  <li><a href="#contact">Nosotros</a></li>
  <li><a href="#about">Contacto</a></li>
  <!-- ¿Cómo colocar a la derecha en menú horizontal? -->
</ul>
```


## Dropdown CSS [ * ](https://www.w3schools.com/css/css_dropdowns.asp)

```css
.dropdown {
    position: relative;
    display: inline-block; /* Ajusta el contenido */
}

.dropdown-content {
    display: none; /* Oculta el contenido */
    position: absolute;
    min-width: 200%; /* Doble del ancho del padre */
    z-index: 1; /* Se muestra por encima */
}

.dropdown:hover .dropdown-content {
    display: block;
}
```


## Dropdown HTML

```html
<div class="dropdown">
  <span>Pasa el <i>mouse</i></span>
  <div class="dropdown-content">
    <p>¡Hola!</p>
  </div>
</div>
```


## Recursos recomendados

* [Bootstrap](http://getbootstrap.com/)
* [Materialize](https://materializecss.com/)
* [Flat UI](http://designmodo.github.io/Flat-UI/)
* [JQuery UI](https://jqueryui.com/)
* [Animate.css](https://daneden.github.io/animate.css/) :star:
* [Font Awesome Free](https://fontawesome.com/free)

## Recomendación

* [UI-Patterns](http://ui-patterns.com/)
* [CSS-Tricks](https://css-tricks.com/)

## Etiquetas `form` e `input`

```html
<form action="destino.php"> <!-- Entorno de formulario -->
  <input> <!-- Elemento de entrada; Cuadro de texto -->
  
  Entrada de texto: <input type="text" name="ejemplo">
  
  <input type="submit" value="Enviar">
  <input type="reset" value="Borrar">
</form>
```


## `method="get|post"`

```html
<form action="destino.php" method="get">
  
  Envía esto desde url:
  <input type="text" name="ejemplo">
  
  Limitado a 3000 caracteres :o
</form>
```

```html
<form action="destino.php" method="post">
  
  Envía esto de manera oculta:
  <input type="text" name="ejemplo">
  
  Sin límite en el tamaño de envío
</form>
```

## `fieldset`

```html
<form action="destino.php">
  
  <fieldset>
    
    <legend>Grupo de datos</legend>
    
    Dato1: <input type="text" name="dato1">
    
    Dato2: <input type="text" name="dato2">
  
  </fieldset>

</form>
```


## Tipos de `input`

```html
<form>
  Texto: <input type="text">
  Correo-e: <input type="email">
  Contraseña: <input type="password">
  
  <input type="radio" name="d1" value="v1"> Val1<br>
  <input type="radio" name="d1" value="v2"> Val2<br>
  
  <input type="checkbox" name="d2" value="v1"> Val1<br>
  <input type="checkbox" name="d2" value="v2"> Val2<br>
  
  <input type="button" onclick="Funcion()" value="Clic">
  
  <input type="submit" value="Enviar">
  <input type="reset" value="Borrar">

  Color: <input type="color">
  
  Fecha: <input type="date">
  Fecha y hora: <input type="datetime-local">
  Tiempo: <input type="time">
  Mes: <input type="month">
  Semana: <input type="week">
  
  Número: <input type="number" min="1" max="5">
  
  Búsqueda: <input type="search">
  URL: <input type="url">
  
  Archivos: <input type="file">
  
  <input type="submit" value="Enviar">
  <input type="reset" value="Borrar">
</form>
```


## Más tipos de `input`

```html
<form id="form1">
  <textarea form="form1" name="val1">
    Área de texto
  </textarea>
  
  <select name="select1">
    <option value="val1">Val1</option>
    <option value="val2">Val2</option>
  </select>
  
  <input type="submit" value="Enviar">
  <input type="reset" value="Borrar">
</form>
```


## Atributos para `input`

```html
<form action="destion.php">
  <input type="text" name="var1" value="Valor desplegado">
  
  <input type="text" name="var2" placeholder="Explicación">
  
  <input value="Requerido" required>
  <input value="Sólo lectura" readonly>
  <input value="Deshabilitado" disabled>
  
  <input value="Empezar aquí" autofocus>
  
  <input value="Otro destino" formaction="destino2.php">
</form>
```

## Tipos de datos Javascript

```javascript
var a; // undefined

var entero = 3; // Number

var flotante = 3.0; // Number

var texto = "Hola"; String

var nula = null; // Equivalente a 0 en operaciones
```

Para imprimir en consola
```javascript
console.log(
  "f12 o ctrl + mayus + i \ 
  abren la consola en Chrome"
); 
```


## Conversión entre tipos de datos

```javascript
var combinado = "Tengo " + 31 + " años.";

var cadena = "7" + 3 // 73

var suma = +"7" + 3 // 10

var textoEntero = parseInt("4")

var textoFlotante = parseFloat("4.5")
```

Convierte a decimal $101_ 2$ y $\text{F}_ {16}$.
```javascript
var aDecimal = parseInt("101", 2)

var aDecimal = parseInt("F", 16)
```


## Operadores

```javascript
var a = 3;

var b = 4;

var c = a + b;
c = a - b;
c = a * b;
c = a / b;

c++;
c += 1;

c = a == b; // Mismo valor
c = a != b; // Valor distinto

c = a === b; // Mismos valor y tipo de dato
c = a !== b; // Distintos valor o tipo de dato
```


## Funciones

```javascript
function SumaDos(a, b){
  var suma = a + b;
  return suma;
}

function Promedio() {
    var suma = 0;
    for (var i = 0, i < arguments.length; i++) {
        suma += arguments[i];
    }
    return suma / arguments.length;
}
```


## Condiciones

```javascript
var a = 3;
if (a == 2) {
  a += 3;
} else if (a < 5) {
  a = 10;
} else {
  console.log(a);
}
```


## Ciclos

```javascript
var a = 0;
while (a < 3) {
  console.log(a);
  a++;
}

for(var i = 0; i < 3; i++){
  console.log(i);
}

var b = 0;
do {
  console.log(b);
  b++;
} while (b < 3)
```


## Arreglos :dog: :cat:

```javascript
var mascotas = new Array();
mascotas[0] = "Pita";
mascotas.push("Toto");
mascotas[2] = "Coqueta";
mascotas.push("Pinto");

for(var i = 0; i < mascotas.length; i++){
  alimentar(mascotas[i]);
}

for(mascota in mascotas){
  querer(mascota);
}
```


## Condiciones de corto circuito :heart:

```javascript
// Si existe un usuario, obtener su nombre
var name = u && u.getName();

// Si no hay asignado un nombre; poner uno por defecto
name = name || "Anónimo";

// Si el nombre es anónimo, no es usuario; lo es
var isUser = (name === "Anónimo") ? false : true;

var a = 1;
switch(a) {
  case 1:
    unaCosa(); // De aquí sigue al 2
  case 2:
    otra();
    break;
  default:
    nada();
}
```


## Objetos

```javascript
// Crear un objeto vacío
var o1 = Object();
var o2 = {};

// Crear un usuario (JSON)
var u = {
  id : 1373079,
  nombre : "Alberto",
  apellido : "Benavides",
  lenguajes : {
    cpp : "90",
    java : "85",
    lens : "75"
  }
}

u.lenguajes.java; // 85
```


## Prototipos (clases)

```javascript
function Usuario(id, nombre){
  this.id = id;
  this.nombre = nombre;
}

var yo = new Usuario(1373079, "Alberto");

var n = yo.nombre;
var mat = yo["id"];

console.log(n);
```


## DOM

* Document Object Module
* Cada elemento HTML es un objeto
* Funciones principales
	* `alert("Muestra una alerta en pantalla");`
	* `console.log("Muestra un mensaje en la consola");`
	* `document.GetElementById("nombreId");`: Obtiene el objeto que lleva por `id` `nombreId`
	* `nombreId`: Equivalente a la instrucción anterior


## Atributos

```javascript
var e = document.GetElementById("elemento");

e.innerHTML; // Contenido del objeto

e.outerHTML; // HTML del elemento; modificarlo lo reemplaza

e.value; // Valor de inputs en formularios
```

## Introducción `jQuery`

* Librería de `javascript`
> "Write less, do more" ([jQuery tutorial](https://www.w3schools.com/jquery/jquery_intro.asp))


## Instalación

* Descargar la librería de [producción](https://code.jquery.com/jquery-3.3.1.min.js)
* Añadirla como archivo externo en `html`
* La fuente puede provenir de un repositorio remoto (p. e. Google)

```html
<head>
  <script src="jquery-3.3.1.min.js"></script>
</head>
```


## Estructura básica

```javascript
// $(selector).acción()

// Elemento más utilizado
$(document).ready(function(){
   // Se ejecuta esta función
   // cuando el documento está listo
});

// Equivalente a la función anterior
$(function(){
   // Contenido a ejecutar
});
```


## Selectores

```javascript
// Todos los párrafos
$("p")

// Todos los vínculos dentro de elementos de lista
$("li a")

// Elemento con id identificador
$("#identificador")

// Elemento con clase clase
$(".clase")

// Todos los párrafos con clase ejemplo
$("p.ejemplo")

// El primer elemento de cualquier lista desordenada
$("ul li:first")
```


## Eventos

```javascript
$(".ejemplo").click();

$(".ejemplo").dblclick();

$(".ejemplo").mouseenter();

$(".ejemplo").mouseleave();

$(".ejemplo").hover();

$("input").focus(); // Cuando se selecciona un input

$("input").blur(); // Cuando se deselecciona un input
```


## Combinación de eventos. Método `on()`

```javascript
// Se utiliza para agrupar eventos para un selector
$("p").on({
  mouseenter: function(){
    $(this).css("background-color", "lightgray");
  }, 
  mouseleave: function(){
    $(this).css("background-color", "lightblue");
  }, 
  click: function(){
    $(this).css("background-color", "yellow");
  } 
});
```


## Obterner valores

```javascript
$("#sel1").click(
  console.log($("#sel2").text()); // innerHTML
  
  console.log($("#sel2").html()); // outerHTML
  
  console.log($("#sel3").val()); // value
  
  // Devuelve el valor del atributo especificado
  console.log($("#sel3").attr("type"));
);
```

## Establecer valores

```javascript
$("#sel1").click(
  $("#sel2").text("Contenido");
  
  $("#sel2").html("<p>Ejemplo</p>");
  
  $("#sel3").val("valor");
  
  // Devuelve el valor del atributo especificado
  $("#sel3").attr("type", "radio");
);
```

Combinación
```javascript
$("#sel1").click(function(){
    $("#vinculo").attr({
        "href" : "www.google.com/",
        "title" : "Google"
    });
});
```


## Añadir

```javascript
$("p").append("Agrega al final del contenido.");

$("p").prepend("Agrega al inicio del contenido.");

$("p").after("Agrega después del elemento.");

$("p").before("Agrega antes del elemento.");

var t1 = "Agrega";
var t2 = "todos";
var t3 = "juntos";

$("p").append(t1, t2, t3);

var e1 = $("<i></i>").text("Crea cursivas");

var e2 = document.createElement("b");
txt3.innerHTML = "Crea negritas";

$("#sel1").before(e1, e2); // Añádelas después de #sel1
```


## Eliminar

```javascript
$("#remover").remove(); // Remueve al elemento y sus hijos

$("#vaciar").empty(); // Remueve los hijos de un elemento

// Remueve párrafos de clase removidos
$("p").remove(".removidos");
```


## `ajax`

* **A**synchronous **J**avaScript **a**nd **X**ML.
* Cargar datos de manera asíncrona (sin que se note)

```javascript
// Sin jQuery
function loadDoc() {
  var xhttp = new XMLHttpRequest();
  xhttp.onreadystatechange = function() {
    if (this.readyState == 4 && this.status == 200) {
      var e = document.getElementById("ejemplo");
      e.innerHtml = this.responseText;
    }
  };
  xhttp.open("GET", "destino.php", true);
  xhttp.send();
}
```

```javascript
// Con jQuery
$(".ejemplo").load("destino.php");
```


## `get` y `post`

```javascript
// $.get(url, datos, funciónFinal);
$.get("destino.php", function(data, status){
  console.log("Datos: " + data);
  console.log("Estado: " + status);
});

// $.post(url, datos, funciónFinal);
$.post("destino.php",
  {
    llave : "valor",
    otraLlave : "otroValor"
  },
  function(data, status){
  	console.log("Datos: " + data);
  	console.log("Estado: " + status);
});
```


## Qué es Java

* Lenguaje orientado a objetos
* Objetos son clases
* Clases son "instructivos"
* Todo es una clase


### Ejemplo :cookie:

* La receta es la **clase**
* Los ingredientes son los **atributos**
* Los pasos son los **métodos**
* La galleta es la **instancia**

```java
public class Galleta {
  float gramosHarina;
  int huevos;
  float mililitrosLeche;
  int cucharadasAzucar;
  
  void MezclarIngredientes(){}
  void Hornear(){}
}

Galleta g = new Galleta();
```


## Instalación de Netbeans

1. Entrar a https://netbeans.org/downloads/
2. Descargar IDE completo (columna derecha)
3. Next, Next, Next, ..., Install


## Instalación JDK (consola)

1. Entrar a http://www.oracle.com/technetwork/java/javase/downloads/index.html
2. Elegir versión SE a descargar (8 es estable)
3. Descargar archivo del sistema operativo


## Estructura mínima programa

```java
// Main.java
// Todo debe estar dentro de una clase
// El archivo debe llevar nombre de la clase
public class Main { // public: Cualquiera puede acceder
  // static: Sin instancia
  public static void main(String[] args) { // Inicio
    System.out.println("Imiprime en consola esta línea");
  }
}
```


## Ejecutar un programa desde NetBeans

1. Abrir NetBeans
* Si hay error de apertura [ * ](https://stackoverflow.com/questions/46476470/cant-create-project-on-netbeans-8-2)
2. File > Create new project
3. Java > Java application > Next
4. Asignar nombre, ubicación, clase main
5. Finish
6. Hacer código
7. Run > Run project


## Ejecutar un programa desde consola

```
rem Compilar el programa
javac Main.java

rem Ejecutar el programa
java Main
```


## Tipos de datos

```java
byte b = 1; // 1 byte

short corto = 1; // 2 bytes

int = entero = 1; // 4 bytes

long largo = 1; // 8 bytes

float flotante = 1; // 4 bytes

double doble = 1; // 8 bytes

char caracter = 1; // 2 bytes

boolean booleano = 1; // 1 byte

// No primitivo
String cadena = new String("1"); // Con constructor

String otraCadena = "1"; // Es lo mismo
```


## Operadores matemáticos

```java
int a = 3;
int b = 4;
int c;

c = a + b;

c = a - b;

c = a * b;

c = a / b;

c = a % b;
```


## Operadores relacionales entre primitivos

```java
int a = 5;
int b = 7;
boolean c;

c = a < b;

c = a > b;

c = a <= b;

c = a >= b;

c = a == b;

c = a != b;
```


## Operadores relacionales con objetos

```java
String s1 = new String("s");
String s2 = "s";
boolean c;

c = s1 == s2; // Falso; son diferentes objetos

c = s1.equals(s2); // Verdadero; tienen el mismo valor
```


## Operadores lógicos

```java
boolean a = true;
boolean b = false;
boolean c;

c = a && b;

c = a || b;
```


## Condicionales

```java
boolean a = true;
boolean b = false;

if (a){ // Si a es verdadero
  // a es verdadero
} else if (b) { // Si no; si b es verdadero
  // a es falso y b verdadero
} else { // Si no
  // a y b son falsas
}

// Ejemplo
if (1 == 1)
  a = true;
else
  a = false;

// Es lo mismo
a = 1 == 1 ? true : false;
```


## Arreglos

```java
// Los arreglos también son objetos D:

int[] arreglo1; // Arreglo de extensión no definida

arreglo1 = new int[5]; // Arreglo de 10 elementos enteros

// Declaración y definición
int[] arreglo2 = new int[5];

// Declaración y definición de elementos
int[] arreglo3 = {1, 2, 3, 4, 5};

arreglo1.length; // Devuelve la cantidad de elementos
```


## Ciclos

```java
for (int i = 0; i < 3; i++) {}

// Equivalente a 

for (;i < 3;) {}

int i = 0;
while (i < 3) {i++;}

i = 0;
do {
  i++;
} while(i < 3);

int[] enteros = {0, 1, 2};
for (int e : enteros){}

// break: Rompre el ciclo
// continue: Continúa con la siguiente iteración
```


## Lectura de datos

```java
import java.util.Scanner;

// [...]

Scanner scanner = new Scanner(System.in);
int a;
String s;

System.out.println("Ingresa un número:");
a = scanner.nextInt();
scanner.nextLine(); // Necesario para evitar saltar línea

System.out.println("Ingresa un texto:");
s = scanner.nextLine();
```


## Funciones y variables globales

```java
public class Main(){

  // tipoDato nombre;

  public static main(){
    // Llamada a funciones
    SinArgumentos();
    ConArgumentos();
  }
  
  public static void SinArgumentos(){}
  
  public static int ConArgumentos(int a, int b){
    return a + b;
  }
}
```


## Correr un programa con argumentos

```java
// Argumentos.java
public class Argumentos(){
  public static void main(String[] args){
    for (;i < args.length;){
      System.out.println(args[i]);
    }
  }
}
```

```
rem Compilar
javac Argumentos.java

rem Ejecutar
java Argumentos arg0 arg1 arg2 ...
```

## POO

* **P**rogramación **O**rientada a **O**bjetos
* Clases como Cajas. Encapsulan:
	* Propiedades estáticas (atributos)
	* Compotamientos dinámicos (métodos)
* Instancia: Objeto de un tipo de clase


## Creación de clases e instancias; atributos

```java
public class PoligonoRegular{
  public String nombre;
  public int lados;
  public float longitud;
  // final siempre declarado
  public final double PI = 3.1415926;
}

PoligonoRegular t1 = new PoligonoRegular();
t1.nombre = "Triángulo equilátero";
t1.lados = 3;
t1.longitud = 1.0;

PoligonoRegular c1;
c1 = new PoligonoRegular();
c1.nombre = "Cuadrado";
c1.lados = 4;
c1.longitud = 1.0;

```


## Métodos, *getters*, *setters*, *this*

```java
public class PoligonoRegular{
  public String nombre;
  int lados; // privados si no se especifica
  private float longitud;
  
  // Getters y Setters (métodos)
  public void SetLados(int n){
    lados = n;
  }
  public int GetLados(){
    return lados;
  }
  public void SetLongitud(float longitud){
    this.longitud = longitud;
  }
  public float GetLongitud(){
    return this.longitud;
  }
}

```


## Constructores, sobrecarga

* Sólo haz variables públicas si hay una buena razón.

```java
public class PoligonoRegular{
  private String nombre;
  private int lados;
  private float longitud;
  
  public PoligonoRegular(){ // Constructor
    this.nombre = "Triángulo";
    this.lados = 3;
    this.longitud = 1.0;
  }
  // Sobrecarga
  public PoligonoRegular(int n, float l){
    this.lados = n;
    this.longitud = l;
  }
}

```


## Método `toString()`

```java
public class PoligonoRegular{
  private String nombre;
  private int lados;
  private float longitud;
  public PoligonoRegular(){
    nombre = "Pentágono";
    lados = 5;
    longitud = 1.0;
  }
  
  public String toString(){
    return nombre + " tiene " + lados +
      " de longitud " + longitud + ".";
  }
  
  PoligonoRegular c1 = new PoligonoRegular();
  System.out.println(c1.toString());
}

```


## Herencia

```java
public class Triangulo{
  public float a, b, c;
  public void SetLados(float a, float b, float c){
    this.a = a;
    this.b = b;
    this.c = c;
  }
}

public class Equilatero extends Triangulo{
  public float h;
  public void SetLados(float a){
    this.a = a;
    this.b = a;
    this.c = a;
    
    this.h = Math.sqrt(c * c - a / 2 * a / 2);
  }
}
```

## Instalar y ejecutar MySQL en Windows

1. Descargar [XAMPP](https://www.apachefriends.org/es/index.html)
2. Abrir XAMPP Control Panel
3. Start en MySQL
4. Shell
5. Correr MySQL con este comando

```cmd
mysql -u <nombreUsuario> -p<contraseña>
```
* Nombre de usuario: `root`
* Contraseña vacía


## Acciones MySQL para bases de datos

```sql
/* Mostrar bases de datos */
show databases;

/* Crear base de datos ejemplo */
create database ejemplo

/* Eliminar base de datos ejemplo */
drop database ejemplo

/* Usar la base de datos ejemplo */
use ejemplo;
```


## Tipos de datos MySQL

* `int`: Entero
* `float(n, d)`: Flotante de $n$ dígitos y $d$ posiciones decimales (incluidas)
* `date`: Fecha en formato AAAA-MM-DD
* `datetime`: Fecha en formato AAAA-MM-DD HH:MM:SS
* `varchar(c)`: Cadena de $c$ caracteres
* `blob`: *Binary Large Object* o Gran objeto binario que suele utilizarse para almacenar multimedia


## Acciones MySQL para tablas

```sql
/* Estructura general */
create table nombreTabla (nombreColumna tipoDato);

/* Crear tabla de usuarios */
create table usuario(
  idUsuario int not null auto_increment, /* Entero++ */
  nombre varchar(50),
  correo varchar(50) unique, /* No permite repetidos */
  claveAcceso varchar(255),
  primary key(id)
);

/* Borrar una tabla */
drop table usuario;

/* Mostrar tablas */
show tables;

/* Mostrar columnas de la tabla usuario */
show columns from usuario;
```


## Añadir registros

```sql
insert into 'usuarios' (
  'nombre', 
  'correo',
  'claveAcceso'
) values (
  'Alberto',
  'bena.87@hotmail.com', 
  sha1('secreta')
);
```


## Llaves foráneas

```sql
create table calificaciones(
  idCalif int not null auto_increment,
  calif float(5, 2),
  idUsuario int,
  primary key (idCalif),
  foreign key (idUsuario) references usuarios(idUsuario)
);
```


## Mostrar registros

```sql
/* Estructura general */
select campo1, campo2, <...>
from tabla1, tabla2, <...>
where condición

/* Todas las columnas y todos los registros de usuarios */
select * from usuarios;

/* Las columas nombre y correo de usuarios */
select nombre, correo from usuarios;

/* Todas las columnas del registro con nombre Alberto */
select * from usuarios where nombre = 'Alberto';
```


## Modificar registros

```sql
/* Estructra general */
update nombreTabla 
set campo1 = nuevoValor1, campo2 = nuevoValor2, <...>
[where condición]

/* Actualizar usuario con id = 1 */
update usuarios
set nombre = 'José', correo = 'otro@correo.com'
where id = 1;
```


## Eliminar registros

```sql
/* Estructura general */
delete from nombreTabla where condición;

/* Eliminar usuario con id = 1 */
delete from usuarios where id = 1;
```


## Ordenar registros

```sql
/* Estructura general */
select campo1, campo2, <...>
from tabla1, tabla2, <...>
order by campo1 asc|desc, campo2 asc|desc;

/* Seleccionar nombres de usuario ordenados por correo */
select nombre from usuarios order by correo asc;
```

## Definición JSP

* JavaServer Pages
* Tecnología de desarrollo web de Java que permite contenido dinámico
* En `HTML` se utilizan estas etiquetas: 
```html
<% etiqueta %>
```


## Requisitos

* [Netbeans](https://netbeans.org/downloads/)
* [JDK](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
* [Extensión de Chrome](https://chrome.google.com/webstore/detail/netbeans-connector/hafdlehgocfcodbgjnpecfajgkeejnaa)


## Crear un proyecto

1. File -> New Project...
2. Categories: Java Web
3. Projects: Web Application. Next
4. Cambiar nombre del proyecto, ubicación. Next
5. Server: Apache... Java version: La más actual
6. Finish
7. Cambiar a Chrome (o Firefox) como navegador principal
8. Play


## Crear un archivo `JSP`

1. Botón derecho en el proyecto
2. New -> JSP...
3. Nombrar `JSP`


## `Java` en `JSP`

```jsp
<%
  // Código Java
%>

<%
  out.println("Texto en pantalla.");
%>

<!-- Comentario ignorado por el navegador -->

<%-- Comentario ignorado por JSP --%>
```


## Librerías, declaración de variables, condiciones

```jsp
<%-- Importar una librería en esta página --%>
<% @page import="java.util.Random" %>
<%-- Declarar una variable --%>
<%! int i = 0; %> 
<% 
Random rand = new Random();
int r = rand.nextInt(10); <%-- [0, 10) --%>
%>

<html> 
  <head><title>Ejemplo</title></head> 
  <body>
    <% if (r % 2 == 0) { %>
      <p> <%= r %> es par.</p>
    <% } else { %>
      <p> <%= r %> es impar.</p>
    <% } %>
  </body> 
</html> 
```


## `switch`

```jsp
<% 
  switch(day) {
    case 0:
      out.println("Cero");
      break;
    case 1:
      out.println("Uno");
      break;
    case 2:
      out.println("Dos");
      break;
    default:
      out.println("Sólo sé contar hasta dos");
      break;
  }
%>
```


## Ciclo `for` y `while`

```jsp
<% for (int i = 0; i < 3; i++){ %>
  <p><%= i %></p>
<% } %>

<%! int i = 0 %>
<% while (i < 3){ %>
  <p><%= i %></p>
  <% i++; %>
<% } %>
```

## *Servlets*

* Intermediarios entre servidores y bases de datos
* Se crean con:
  1. Botón derecho en proyecto
  2. New -> Servlet...
  3. Especificar Class Name; Next
  4. Especificar nombre y url; Finish


## Método `processRequest` de un *servlet*

```java
// Procesa la petición de la url especificada
protected void processRequest
  // Atributos de petición y respuesta
  (HttpServletRequest request,HttpServletResponse response)
  throws ServletException, IOException {
  
  // Tipo de contenido de la respuesta
  response.setContentType("text/html;charset=UTF-8");
  
  // Declarar atributos y valores del 
  request.setAttribute("mensaje", "Hola");
  
  // Retornar ejemplo.jsp
  request.getRequestDispatcher("/ejemplo.jsp").
    forward(request, response);
}
```


## *Servlet* `ejemplo.jsp`

```jsp
<%@page contentType="text/html" pageEncoding="UTF-8"%>
<!DOCTYPE html>
<html>
  <head>
    <meta http-equiv="Content-Type" content="text/html; 
      charset=UTF-8">
    <title>Ejemplo</title>
  </head>
  <body>
    <!-- Obtiene el atrubuto mensaje -->
    <h1><%= request.getAttribute("mensaje") %></h1>
  </body>
</html>
```


## Método `doGet` de un *servlet*

```java
@Override
// Definición del método para recibir peticiones get
protected void doGet
  (HttpServletRequest request,HttpServletResponse response)
  throws ServletException, IOException {
  response.setContentType("text/html;charset=UTF-8");

  // Recepción de parámetros
  String nombre = request.getParameter("nombre");
  int edad = Integer.parseInt(
      request.getParameter("edad")
    );
  
  request.setAttribute("nombre", nombre);
  request.setAttribute("edad", edad);
  request.getRequestDispatcher("/mostrarInfo.jsp").
    forward(request, response);
}
```


## *Servlet* `mostrarInfo.jsp`

```jsp
<%@page contentType="text/html" pageEncoding="UTF-8"%>
<!DOCTYPE html>
<html>
  <head>
    <meta http-equiv="Content-Type" content="text/html; 
      charset=UTF-8">
    <title>Usuarios</title>
  </head>
  <body>
    <h1>Ejemplo</h1>
    <p>Nombre: <%= request.getAttribute("nombre") %></p>
    <p>Edad: <%= request.getAttribute("edad") %></p>
  </body>
</html>
```


## *Servlet* `formulario.jsp`

```jsp
<!DOCTYPE html>
<html>
  <body>
    <form action = "info" method = "POST">
      Nombre: <input type = "text" name = "nombre">
      <br />
      Edad: <input type = "number" name = "edad" />
      <input type = "submit" value = "Enviar" />
    </form>
  </body>
</html>
```


## Método `doPost` de un *servlet*

```java
// Definición del método para recibir peticiones post
@Override
protected void doPost
  (HttpServletRequest request,HttpServletResponse response)
  throws ServletException, IOException {
  response.setContentType("text/html;charset=UTF-8");

  String nombre = request.getParameter("nombre");
  int edad = Integer.parseInt(
      request.getParameter("edad")
    );
  
  request.setAttribute("nombre", nombre);
  request.setAttribute("edad", edad);

  request.getRequestDispatcher("/mostrarInfo.jsp").
    forward(request, response);
}
```

# Fuentes

* https://developer.mozilla.org/es/docs/Learn/HTML/Introduccion_a_HTML/iniciar 
* https://www.w3.org/MarkUp/Guide/ 
* https://www.w3schools.com/html/html_intro.asp 
* https://developer.mozilla.org/es/docs/Learn/HTML/Introduccion_a_HTML/iniciar 
* https://www.w3.org/MarkUp/Guide/ 
* https://www.w3schools.com/html/html_intro.asp 
* https://www.w3schools.com/css/default.asp
* https://www.w3.org/Style/Examples/011/firstcss.es.html
* https://www.w3schools.com/html/html_forms.asp
* https://www.w3schools.com/js/
* https://developer.mozilla.org/es/docs/Web/JavaScript/Guide/Introducci%C3%B3n
* https://developer.mozilla.org/es/docs/Web/JavaScript/Una_re-introducci%C3%B3n_a_JavaScript
* https://javascript.info/
* https://www.w3schools.com/jquery/jquery_intro.asp
* https://jquery.com/
* https://www.learnjavaonline.org/
* https://docs.oracle.com/javase/tutorial/getStarted/cupojava/index.html
* http://www.ntu.edu.sg/home/ehchua/programming/java/J3a_OOPBasics.html
* https://www.learnjavaonline.org/en/Inheritance
* https://www.tutorialspoint.com/java/number_sqrt.htm
* https://www.tutorialspoint.com/mysql/index.htm
* https://zinoui.com/blog/storing-passwords-securely
* https://www.w3schools.com/Sql/sql_foreignkey.asp
* https://www.tutorialspoint.com/jsp/jsp_syntax.htm
* https://www.tutorialspoint.com/servlets/servlets-form-data.htm
* https://stackoverflow.com/questions/6452537/servlet-send-response-to-jsp