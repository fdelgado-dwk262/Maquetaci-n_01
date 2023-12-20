# Maquetacion_06
## Ejercicios Maquetación

### Axpe Consulting - Front
 Ejercicios HTML / CSS
 
## Introducción

Creamos un "Arbol de Navidad" con css y html

Ejemplo sobre Vscode, pero se puede montar sobre cualquier editor.

## Estructura básica de HTML

Crearemos un ficheo index.html 

En el cual ( desde vscode ) teclearemos y pulsaremos intro

```html
html:5
```

y nos genrea de forma automática ya la primera estructura base para poder empezar a tabajar

No obstante desde cualquier editor, podemos usar :

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>
```

En el body del nuestro html crearemos la siguiente structura, la cual estará dividida en varias partes 
la parte princila el arbol y el tronco, dentro de la parte del arbol, tendremos las "ramas" y la decoración

```html
        <div class="xmas">
            <div class="tree">
                <div class="ball">
                    <div class="ball-1"></div>
                    <div class="ball-2"></div>
                    <div class="ball-3"></div>
                    <div class="ball-4"></div>
                    <div class="ball-5"></div>
                    <div class="ball-6"></div>
                    <div class="ball-7"></div>
                    <div class="ball-8"></div>
                    <div class="ball-9"></div>
                </div>
                <div class="tree-1"></div>
                <div class="tree-2"></div>
                <div class="tree-3"></div>
                <div class="tree-4"></div>
                <div class="tree-5"></div>
                <div class="tree-6"></div>
                <div class="tree-7"></div>
                <div class="tree-8"></div>
            </div>
            <div class="trunk"></div>
        </div>
```

## En el apartado del CSS 

Dejo el css sacado directamente desde SASSMEINSTER y su versión SCSS
y poosterior mente mnodificado para ver diferentes temas.

```css
:root {
  --shadow-color: 94deg 100% 14%;
  --shadow: 0.3px 0.4px 0.6px hsl(var(--shadow-color) / 0.34),
  	1.7px 2.3px 3.2px -0.4px hsl(var(--shadow-color) / 0.34),
  	3.2px 4.4px 6.1px -0.7px hsl(var(--shadow-color) / 0.34),
  	5.3px 7.2px 10.1px -1.1px hsl(var(--shadow-color) / 0.34),
  	8.5px 11.5px 16.1px -1.4px hsl(var(--shadow-color) / 0.34),
  	13.2px 18px 25.1px -1.8px hsl(var(--shadow-color) / 0.34),
  	20.1px 27.3px 38.1px -2.1px hsl(var(--shadow-color) / 0.34),
  	29.6px 40.2px 56.2px -2.5px hsl(var(--shadow-color) / 0.34);
}

.tree-1 {
  width: 60px;
  height: 50px;
}

.ball-1 {
  --ball-size: 40px;
  width: var(--ball-size);
  height: var(--ball-size);
  border-radius: 50px;
  position: absolute;
}

.tree-2 {
  width: 120px;
  height: 50px;
}

.ball-2 {
  --ball-size: 40px;
  width: var(--ball-size);
  height: var(--ball-size);
  border-radius: 50px;
  position: absolute;
}

.tree-3 {
  width: 180px;
  height: 50px;
}

.ball-3 {
  --ball-size: 40px;
  width: var(--ball-size);
  height: var(--ball-size);
  border-radius: 50px;
  position: absolute;
}

.tree-4 {
  width: 240px;
  height: 50px;
}

.ball-4 {
  --ball-size: 40px;
  width: var(--ball-size);
  height: var(--ball-size);
  border-radius: 50px;
  position: absolute;
}

.tree-5 {
  width: 300px;
  height: 50px;
}

.ball-5 {
  --ball-size: 40px;
  width: var(--ball-size);
  height: var(--ball-size);
  border-radius: 50px;
  position: absolute;
}

.tree-6 {
  width: 360px;
  height: 50px;
}

.ball-6 {
  --ball-size: 40px;
  width: var(--ball-size);
  height: var(--ball-size);
  border-radius: 50px;
  position: absolute;
}

.tree-7 {
  width: 420px;
  height: 50px;
}

.ball-7 {
  --ball-size: 40px;
  width: var(--ball-size);
  height: var(--ball-size);
  border-radius: 50px;
  position: absolute;
}

.tree-8 {
  width: 480px;
  height: 50px;
}

.ball-8 {
  --ball-size: 40px;
  width: var(--ball-size);
  height: var(--ball-size);
  border-radius: 50px;
  position: absolute;
}

.tree div:nth-child(4n+1) {
  background: #2d6359;
  box-shadow: var(--shadow);
}

.ball div:nth-child(4n+1) {
  background: #e388b1;
  box-shadow: var(--shadow);
}

.tree div:nth-child(4n+2) {
  background: #32776a;
  box-shadow: var(--shadow);
}

.ball div:nth-child(4n+2) {
  background: #f4d348;
  box-shadow: var(--shadow);
}

.tree div:nth-child(4n+3) {
  background: #268b4c;
  box-shadow: var(--shadow);
}

.ball div:nth-child(4n+3) {
  background: #37799e;
  box-shadow: var(--shadow);
}

.tree div:nth-child(4n+4) {
  background: #459763;
  box-shadow: var(--shadow);
}

.ball div:nth-child(4n+4) {
  background: #bb3e39;
  box-shadow: var(--shadow);
}

body {
  background-color: beige;
}

.xmas,
.tree {
  display: flex;
  align-items: center;
  flex-direction: column;
}

.xmas {
  margin: 6rem 0 0 0;
}

.star {
  position: relative;
  z-index: 2;
}

.tree {
  position: relative;
}

.trunk {
  --trunk: #9e6328;
  width: 50px;
  height: 50px;
  background-color: var(--trunk);
  box-shadow: var(--shadow);
}

.ball-1 {
  left: 250px;
  top: 80px;
}
.ball-2 {
  left: 150px;
  top: 230px;
}
.ball-3 {
  left: 300px;
  top: 230px;
}
.ball-4 {
  left: 80px;
  top: 310px;
}
.ball-5 {
  left: 200px;
  top: 280px;
}
.ball-6 {
  left: 360px;
  top: 330px;
}
.ball-7 {
  left: 170px;
  top: 120px;
}
.ball-8 {
  left: 244px;
  top: 173px;
}
```
## SCSS

```scss
:root {
	--shadow-color: 94deg 100% 14%;
	--shadow: 0.3px 0.4px 0.6px hsl(var(--shadow-color) / 0.34),
		1.7px 2.3px 3.2px -0.4px hsl(var(--shadow-color) / 0.34),
		3.2px 4.4px 6.1px -0.7px hsl(var(--shadow-color) / 0.34),
		5.3px 7.2px 10.1px -1.1px hsl(var(--shadow-color) / 0.34),
		8.5px 11.5px 16.1px -1.4px hsl(var(--shadow-color) / 0.34),
		13.2px 18px 25.1px -1.8px hsl(var(--shadow-color) / 0.34),
		20.1px 27.3px 38.1px -2.1px hsl(var(--shadow-color) / 0.34),
		29.6px 40.2px 56.2px -2.5px hsl(var(--shadow-color) / 0.34);
}

@for $i from 1 through 8 {
	.tree-#{$i} {
		width: 60px * $i;
		height: 50px;
	}
	.ball-#{$i} {
		--ball-size: 40px;
		width: var(--ball-size);
		height: var(--ball-size);
		border-radius: 50px;
		position: absolute;
	}
}

$colors: #0d1d1a, #142f2a, #103b20, #255135;
$balls: #e388b1, #f4d348, #37799e, #bb3e39;

@for $i from 1 through length($colors) {
	.tree div:nth-child(#{length($colors)}n + #{$i}) {
		background: lighten(nth($colors, $i), 20%);
		box-shadow: var(--shadow);
	}
	.ball div:nth-child(#{length($balls)}n + #{$i}) {
		background: (nth($balls, $i));
		box-shadow: var(--shadow);
	}
}

body {
	background-color: beige;
}
.xmas,
.tree {
	display: flex;
	align-items: center;
	flex-direction: column;
}

.xmas {
	margin: 6rem 0 0 0;
}

.star {
	position: relative;
	z-index: 2;
}

.tree {
	position: relative;
}
.trunk {
	--trunk: #9e6328;
	width: 50px;
	height: 50px;
	background-color: var(--trunk);
	box-shadow: var(--shadow);
}

.ball {
	&-1 {
		left: 250px;
		top: 80px;
	}
	&-2 {
		left: 150px;
		top: 230px;
	}
	&-3 {
		left: 300px;
		top: 230px;
	}
	&-4 {
		left: 80px;
		top: 310px;
	}
	&-5 {
		left: 200px;
		top: 280px;
	}
	&-6 {
		left: 360px;
		top: 330px;
	}
	&-7 {
		left: 170px;
		top: 120px;
	}
	&-8 {
		left: 244px;
		top: 173px;
	}
}

```

## Pseudeselector
Un pseudeselector es una instrucción que acompaña un selector para añadir un aspecto decorativo a un elemento.
En esta entrada trataremos ::before y ::after.

Un pseudoselector no es exactamente que una pseudoclase. Mientras que el pseudoselector atiende al aspecto estético, la pseudoclase atiende al estado del elemento. Un ejemplo de pseudoclase es :hover.
Actualmente el W3C insiste en que pongamos 2 veces 2 puntos para diferenciar los pseudoselectores de las pseudoclases.
::before y ::after se suelen usar con la instrucción content. También pueden ir acompañadas de otras instrucciones como margin o padding.

Es importante que tengas en cuenta que el elemento añadido será un elemento en línea.

Recuerda que los elementos en línea no tienen width, height, ni margin-top ni margin-bottom.

En función de lo que quieras hacer deberás combinarlo con display:block; o display:inline-block.

Vemos un ejemplo en este mismo ejemplo en la estrella que corona nuestro arbol.

## Constantes
Llamadas variables dentro del CSS, son nativas y se definen al principio de nuestra hoja de estilos y se usa de la siguiente forma.

Nota .- se puede definir una variable dentro de una clase, si se puede pero se usará dentro de esta clase, esto recuerda a JS, este falor no tomara el de ámbito global sino su valor local.

Por otro lado es conveniente usalr un valor por defecto si un navegador no interpretase el valor de la constante.

```css
:root {
   --definicion-de-variable: valor;
   
   --color-bg: #f3f3f3;
}
.clase {
   color: var(--color-bg, #f3f3f3);
}

.clase-sobreescrita {
   --color-bg: red;
   color: var(--color-bg, #f3f3f3);
}

```

##
##

## Url's de referencia .- 
* [the-shapes-of-css](https://css-tricks.com/the-shapes-of-css/)
* [formas-basicas-con-css](https://cybmeta.com/formas-basicas-con-css-triangulos-circulos-trapecios-rectangulos-cuadrados)
* [css3-estrella](https://www.sessionstudio.com.ar/blog/2011/02/22/formas-en-css3-estrella/)
* [orden-de-las-propiedades-css](https://raohmaru.com/blog/css/el-orden-de-las-propiedades-css/)
* [sassmeister](https://www.sassmeister.com/)
* [makeareadme](https://www.makeareadme.com/)
* [specificity](https://specificity.keegan.st/)
* [CSS selectores y propiedades ( a-z ) ](https://css-tricks.com/almanac/)

##
No necesitamos instalacion ni servidor alguno para este ejemplo