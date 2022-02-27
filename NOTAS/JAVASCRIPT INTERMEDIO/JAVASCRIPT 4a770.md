# JAVASCRIPT INTERMEDIO

# Booleans y condicionales

### Booleano

El objeto **`Boolean`** es un objeto contenedor para un valor booleano.

![Untitled](JAVASCRIPT%204a770/Untitled.png)

**Ejemplo:**

![Untitled](JAVASCRIPT%204a770/Untitled%201.png)

Veremos como retorna un valor que sale de una expresion

![Untitled](JAVASCRIPT%204a770/Untitled%202.png)

![Untitled](JAVASCRIPT%204a770/Untitled%203.png)

![Untitled](JAVASCRIPT%204a770/Untitled%204.png)

El triple igual en JS además de verificar el valor, verifica el tipo.

![Untitled](JAVASCRIPT%204a770/Untitled%205.png)

---

# Loops: for, while y forEach

### **Loops:**

Formas de repetir tareas

Array Push

El método **`push()`**añade uno o más elementos al final de un array y devuelve la nueva longitud del array.

![Untitled](JAVASCRIPT%204a770/Untitled%206.png)

![Untitled](JAVASCRIPT%204a770/Untitled%207.png)

![Untitled](JAVASCRIPT%204a770/Untitled%208.png)

La tarea anterior de añadir elementos al array se hace muy repetitiva, para ello utilizaremos loops.

```jsx
let miArray =[];
for(let i=0; i<10; i=i+1){
  miArray.push(i);
}

miArray
```

![Untitled](JAVASCRIPT%204a770/Untitled%209.png)

---

### **While**

```jsx

let miArray2= []
let control = 0;
while(control< 10){
miArray2.push(control);
control = control+1
}
miArray2
```

![Untitled](JAVASCRIPT%204a770/Untitled%2010.png)

Otro Ejemplo de uso de while

![Untitled](JAVASCRIPT%204a770/Untitled%2011.png)

typeof Array

![Untitled](JAVASCRIPT%204a770/Untitled%2012.png)

![Untitled](JAVASCRIPT%204a770/Untitled%2013.png)

---

### **ForEach**

El método **`forEach()`**ejecuta la función indicada una vez por cada elemento del array.

El forEach no devuelve nada, si queremos ver la salida debemos poner un console log

**JavaScript Demo: Array.forEach() a continuacion:**

```jsx
const array1 = ['a', 'b', 'c'];

array1.forEach(element => console.log(element));

// expected output: "a"
// expected output: "b"
// expected output: "c"
```

```jsx
let miArray = ['hola' , 'buen dia', 'adios'];

function convertirMayusculas(texto){
	return texto.toUpperCase();
}
convertirMayusculas('fegegregegre');

// expected output:FEGEGREGRGRE
```

El **`toUpperCase()`**método devuelve el valor convertido en mayúsculas de la cadena que realiza la llamada.

![Untitled](JAVASCRIPT%204a770/Untitled%2014.png)

![Untitled](JAVASCRIPT%204a770/Untitled%2015.png)

---

### Array.map

El método **`map()`**crea un nuevo array con los resultados de la llamada a la función indicada aplicados a cada uno de sus elementos.

```jsx
var numbers = [1, 5, 10, 15];
var doubles = numbers.map(function(x) {
   return x * 2;
});

```

![Untitled](JAVASCRIPT%204a770/Untitled%2016.png)

son parecidos al forEach pero el forEach no entrega ningun retorno

---

### Array.filter

Me devuelve un array con los elementos cuya condicion  del retorno de la funcion que le pase al filter sea verdadera

![Untitled](JAVASCRIPT%204a770/Untitled%2017.png)

---

### Arrow functions (funciones de flecha)

```jsx
function miFuncion2(){
	console.log('ejecute miFuncion2')
}

```

```jsx
function miFuncion(){
	console.log('1 ejecuta miFuncion')
	console.log('2 ejecute miFuncion')
	miFuncion2()
}
```

![Untitled](JAVASCRIPT%204a770/Untitled%2018.png)

![Untitled](JAVASCRIPT%204a770/Untitled%2019.png)

La forma anterior es la ejecución de una función. A continuación voy a convertir las funciones en arrow functions

```jsx
const miFuncion2 = ()=>{
	console.log('ejecuta miFuncion2')
}
```

Las `Arrow Functions` tienen otra particularidad:

```jsx
console.log(miFuncion())

function miFuncion(){
	return 100
}
```

La segunda parte del Código en la imagen vendría siendo la primera parte, después de que JS lo compila.

![Untitled](JAVASCRIPT%204a770/Untitled%2020.png)

Las Arrow Functions no se pueden acceder antes de su definicion

```jsx
console.log(miFuncion())
 const miFuncion = () =>{
     return 100
 }
```

![Untitled](JAVASCRIPT%204a770/Untitled%2021.png)

## Scope

El scope de una variable hace referencia al lugar donde esta va a vivir , o podrá ser accesible.

Podríamos decir también que scope es el alcance que determina la accesibilidad de las variables en cada parte de nuestro código.

El objeto window es un ejemplo de scope global.

![Untitled](JAVASCRIPT%204a770/Untitled%2022.png)

![Untitled](JAVASCRIPT%204a770/Untitled%2023.png)

Ahora veremos el ejemplo donde el`scope` es `window` cuando usamos una Arrow Function

![Untitled](JAVASCRIPT%204a770/Untitled%2024.png)

---

## Comportamientos de arrow functions comparados con las funciones normales

Comparación con ejemplos:

Función

![Untitled](JAVASCRIPT%204a770/Untitled%2025.png)

Arrow Function

![Untitled](JAVASCRIPT%204a770/Untitled%2026.png)

![Untitled](JAVASCRIPT%204a770/Untitled%2027.png)

![Untitled](JAVASCRIPT%204a770/Untitled%2028.png)

Crear un objeto a partir de la función 5

![Untitled](JAVASCRIPT%204a770/Untitled%2029.png)

![Untitled](JAVASCRIPT%204a770/Untitled%2030.png)

En este caso el this que retorna es el método

![Untitled](JAVASCRIPT%204a770/Untitled%2031.png)

Arrow Function

![Untitled](JAVASCRIPT%204a770/Untitled%2032.png)

En JavaScript podemos crear las funciones dentro de los objetos sin necesidad de poner la palabra Function.

![Untitled](JAVASCRIPT%204a770/Untitled%2033.png)

Hay diferencias de una función dentro de un objeto con respecto a una Arrow Function dentro de un objeto.

![Untitled](JAVASCRIPT%204a770/Untitled%2034.png)

Hay que tener cuidado con esto

![Untitled](JAVASCRIPT%204a770/Untitled%2035.png)

> Cuando utilizo Arrow Functions y cuando utilizo Funciones normales dependiendo de donde estén declaradas y de a donde las este usando esas Arrows Functions y esas funciones cambian de scope. Hay que tener eso presente.
> 

![Untitled](JAVASCRIPT%204a770/Untitled%2036.png)

---

# **Destructuring (destructuración)**

Cualidad que se le agrego a JS en ECMAScript v6

**ECMAScript v6**
Es el estándar que sigue JavaScript desde Junio de 2015. Hasta ese momento la versión de JS que estábamos usando en nuestros navegadores y Node.js, era la v5.

Ahora hasta el momento vamos por ECMAScript 2022.

D**estructuración:**

Es algo para trabajar con objetos y Arrays de una manera mas simple, mas elegante. La **destructuración** puede hacerse en Arrays tanto como en objetos.

Ejemplo:

```jsx
let miObjeto = {a:1, b:2, c:'hola' , 
								d: function(){console.log('soy una funcion')},
							  e:true}
```

![Untitled](JAVASCRIPT%204a770/Untitled%2037.png)

La destructuracion es acceder o desaclopar ese objeto envariables mas simples. Si necesito trabajar con esas propiedades en un futuro , o con algunas partes de ese objeto pues simplemente lo destructuro. De la siguiente forma:

![Untitled](JAVASCRIPT%204a770/Untitled%2038.png)

Destructuracion de un Array.

Podemos hacer lo anterior con un Array tambien

```jsx
let miArray = [1,  2, 'hola' , ()=> console.log('Soy Funcion'), true]
```

![Untitled](JAVASCRIPT%204a770/Untitled%2039.png)

Si yo quiero excluir un elemento del objeto puedo hacer lo siguiente

![Untitled](JAVASCRIPT%204a770/Untitled%2040.png)

![Untitled](JAVASCRIPT%204a770/Untitled%2041.png)

Mutacion de un Objeto

![Untitled](JAVASCRIPT%204a770/Untitled%2042.png)

---

# Destructuring (destructuración) clonación profunda y superficial

### Lodash

**Una moderna biblioteca de utilidades de JavaScript que ofrece modularidad, rendimiento y extras**

Haciendo una copia profunda de mi objeto.

![Untitled](JAVASCRIPT%204a770/Untitled%2043.png)

 

![Untitled](JAVASCRIPT%204a770/Untitled%2044.png)

---

# Prototype (prototipo)

Los prototipos son un enlace , una propiedad de los objetos en JavaScript

```jsx
function MiObjeto(nombre, apellido){
	this.nombre= nombre
	this.apellido = apellido
	this.getNombreCompleto = function(){
		return `${this.nombre} ${this.apellido}`
	} 
}
```

![Untitled](JAVASCRIPT%204a770/Untitled%2045.png)

Comparación entre objeto y JSON

![Untitled](JAVASCRIPT%204a770/Untitled%2046.png)

Prototype

![Untitled](JAVASCRIPT%204a770/Untitled%2047.png)

![Untitled](JAVASCRIPT%204a770/Untitled%2048.png)

Podemos Settear los parametros de un objeto, quedan el el prototipo.

![Untitled](JAVASCRIPT%204a770/Untitled%2049.png)

![Untitled](JAVASCRIPT%204a770/Untitled%2050.png)

![Untitled](JAVASCRIPT%204a770/Untitled%2051.png)

Los prototipos son un mecanismo mediante el cual los objetos en JavaScript heredan características entre sí.

## [¿Un lenguaje basado en prototipos?](https://developer.mozilla.org/es/docs/Learn/JavaScript/Objects/Object_prototypes#%C2%BFun_lenguaje_basado_en_prototipos)

JavaScript es a menudo descrito como un **lenguaje basado en prototipos -** para proporcionar mecanismos de herencia, los objetos pueden tener un **objeto prototipo**, el cual actúa como un objeto plantilla que hereda métodos y propiedades.

Un objeto prototipo del objeto puede tener a su vez otro objeto prototipo, el cual hereda métodos y propiedades, y así sucesivamente. Esto es conocido con frecuencia como la **cadena de prototipos**, y explica por qué objetos diferentes pueden tener disponibles propiedades y métodos definidos en otros objetos.