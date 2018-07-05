# ¿Qué es una función?

Una función es una porción de código encapsulada que se puede nombrar y reutilizar cuando quiera cuantas veces quiera.

Las funciones son el principal mecanismo de scope.

## Declarar una función
Para declarar una función utilizamos la palabra reservada *function* seguida de *()*, seguidos de *{}*
Más claramente:

```js 
function () {
	// código que quiero ejecutar
}

```

Una función puede recibir 0 o más parámetros o argumentos, de la siguiente manera:

```js
function (parametros, separados, por, coma) {
	// código que quiero ejecutar
}
```

Una función puede devolver o no un valor. Para devolver un valor usamos la palabra reservada *return*.

```js
function (parametros, separados, por, coma) {
	// código que quiero ejecutar

	return 'Un valor que quiero devolver';
}
```

Las anteriores son funciones anónimas. Las funciones pueden tener nombre.

```js 
function soyUnaFuncion() {
	// código que quiero ejecutar
}

```

Y pueden ser asigandas como valor con o sin nombre:
```js 
var soyUnaFuncion = function () {
	// código que quiero ejecutar
}

// esta es la manera más corriente de declarar una función.
```
o 

```js 
var soyUnaFuncion = function esteEsMiNombre() {
	// código que quiero ejecutar
}

```

## Ejecutar una función
Para correr el código que guardé en mi función tengo que ejecutarla. Para esto tengo que llamar a mi función seguida de *()*

```js 
var soyUnaFuncion = function () {
	// código que quiero ejecutar
}

soyUnaFuncion()
```

Cuando ejecuto una función puedo pasarle los parámetros

```js 
var soyUnaFuncion = function (arg1, arg2, arg3) {
	console.log(arg1, arg2, arg3); 
}

soyUnaFuncion('hola', 3, [1,2,3]) // 'hola', 3, [1, 2, 3]

```

Puede ejecutar una función la cantidad de veces que quiera, pasándole los parámetros que quiera

```js 
var soyUnaFuncion = function (numA, numB) {
	var b = numA + numB;
	console.log(b); 
}

soyUnaFuncion(1, 1) // 2
soyUnaFuncion(10, 105) // 115
soyUnaFuncion(3, 4) // 7
soyUnaFuncion(10203, 1) // 10204
soyUnaFuncion(5, 3) // 8
```
La función es siempre la misma, actúa de template.

