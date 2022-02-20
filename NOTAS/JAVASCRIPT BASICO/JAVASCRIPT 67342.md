# JAVASCRIPT BASICO

## Variables:

 Espacio en memoria donde yo guardo valores .Var es una palabra reservada del lenguaje

```jsx
var curso = 'Aprendiendo JavaScript' 
```

Undefined: indefinido

```jsx
var minumero = 6
var r 
```

Paso de referencia

la referencia de r es undefined. Cuando no le digo que referencia debe de guardar siempre sera undifined

```jsx
curso = r
```

![Untitled](JAVASCRIPT%2067342/Untitled.png)

Error de referencia

```jsx
curso = bootcamp
```

![Untitled](JAVASCRIPT%2067342/Untitled%201.png)

Al redeclarar una variable ocurre un undefined.

---

## Primitivas String y number Parte 2

Si no quiero redefinir el valor de una variable, usare una constante

```jsx
const curso = 'Ingenieria de Software'
```

![Untitled](JAVASCRIPT%2067342/Untitled%202.png)

Tipo de varible LET

![Untitled](JAVASCRIPT%2067342/Untitled%203.png)

Puedo redefinir la variable con  let

Existen 3 formas de declarar una variable:

- Let
- var
- const

Variables  para almacenar números / operaciones con numeros

![Untitled](JAVASCRIPT%2067342/Untitled%204.png)

Concatenación

![Untitled](JAVASCRIPT%2067342/Untitled%205.png)

String Literal

![Untitled](JAVASCRIPT%2067342/Untitled%206.png)

[JavaScript | MDN](https://developer.mozilla.org/es/docs/Web/JavaScript)

---

## Primitivas String y number Parte 3

Existen 7 tipos de variables en JS, y es bajamente tipado

![Untitled](JAVASCRIPT%2067342/Untitled%207.png)

**Operador Typeof** 

![Untitled](JAVASCRIPT%2067342/Untitled%208.png)

En JS no hay diferencia entre tipos de números, todos son numeros.

![Untitled](JAVASCRIPT%2067342/Untitled%209.png)

---

## Object y null

![Untitled](JAVASCRIPT%2067342/Untitled%2010.png)

Que otros valores pueden existir en JavaScript a parte de numeros, cadenas..?

Pueden haber objetos, cuya notación es con llaves

```jsx
let object = {}
```

![Untitled](JAVASCRIPT%2067342/Untitled%2011.png)

Los objetos pueden tener variables por dentro, a estas variables les llamamos propiedades.

```jsx
let objeto1={propiedad1:'text1'}
```

Para acceder a las propiedades de un objeto podemos acceder con la notación de punto

![Untitled](JAVASCRIPT%2067342/Untitled%2012.png)

propiedad1 tiene tipo, asi que tambien puedo saberlo

![Untitled](JAVASCRIPT%2067342/Untitled%2013.png)

Al objeto1 puedo agregarle números

![Untitled](JAVASCRIPT%2067342/Untitled%2014.png)

Yo puedo tener objetos dentro de un objeto

![Untitled](JAVASCRIPT%2067342/Untitled%2015.png)

Primitivas en JS

- Objetos
- Cadenas de texto
- Números

Tambien hay otros tipos de primitivas

- **Valor null:** La característica mas particular de null, es que typeof null retorna object. Es un bug
    
    ![Untitled](JAVASCRIPT%2067342/Untitled%2016.png)
    

- **Undefined**:
    
    ![Untitled](JAVASCRIPT%2067342/Untitled%2017.png)
    

- **Booleanos**:
    
    ![Untitled](JAVASCRIPT%2067342/Untitled%2018.png)
    
    Cuando una variable no esta definida su variable es *undefined* por defecto.
    
    ![Untitled](JAVASCRIPT%2067342/Untitled%2019.png)
    

- **Symbol():**
    
    ![Untitled](JAVASCRIPT%2067342/Untitled%2020.png)
    

### Expresiones

Puede ser mas fácil de identificar cuando estoy declarando una variable y de una vez la estoy inicializando.

```jsx
let var
const nombreVariable = 1
```

Una **expresión** es el lado derecho del igual, es algo que el lenguaje me entiende pero no puedo ejecutar operaciones con esa linea de Código.

![Untitled](JAVASCRIPT%2067342/Untitled%2021.png)

---

---

## JSON y el objeto window

¿Que es un JSON?

Notación de objeto estándar para casi todas las aplicaciones.

**J**ava**S**cript **O**bject **N**otation 

Los objetos son un tipo de valor muy importante dentro de los lenguajes de programación.

![Untitled](JAVASCRIPT%2067342/Untitled%2022.png)

Hay dos objetos muy importantes que el motor de JS que vive dentro de un navegador tiene

1. **Window**
    
    window tiene un montón de propiedades que son necesarias para el desarrollador en el lado del navegador. 
    
    Ejemplo: Document, History, navigator y muchos mas.
    
    ![Untitled](JAVASCRIPT%2067342/Untitled%2023.png)
    
    ![Untitled](JAVASCRIPT%2067342/Untitled%2024.png)
    
    Propiedad width
    
    ![Untitled](JAVASCRIPT%2067342/Untitled%2025.png)
    
    Para ver cuanto ancho mide la parte visual donde se renderiza la pagina.
    
    Su propip ancho
    
    ![Untitled](JAVASCRIPT%2067342/Untitled%2026.png)
    
    window es el valor por defecto en donde esta parado la consola de JS cuendo la abrimos.
    

---

## Window, alert, document

Hay una propiedad que es muy usada y sirve para lanzar un mensaje, es la propiedad alert. Hare mi hello world con alert

```jsx
alert('Hello Word')
```

![Untitled](JAVASCRIPT%2067342/Untitled%2027.png)

Nos entrega una caja de texto con el mensaje que le pasamos, y esa es a su vez algo de window

```jsx
window.alert('Hello World')
```

![Untitled](JAVASCRIPT%2067342/Untitled%2027.png)

**SCOPE**

Ámbito, contexto. Va a ser super importante porque querremos saber el SCOPE, el ámbito o el contexto en donde estamos parados en el momento.

Objeto Document

Representación de todo el HTML que tiene la pagina dentro de un objeto de JS. Document normalmente solo lo vamos a encontrar en navegadores.

![Untitled](JAVASCRIPT%2067342/Untitled%2028.png)

Document es una API es un recurso que los navegadores le agregan al JS.

Document esta dentro de window

![Untitled](JAVASCRIPT%2067342/Untitled%2029.png)

![Untitled](JAVASCRIPT%2067342/Untitled%2030.png)

---

---

## Nesting (anidamiento) y scope (alcance)

Document: 

Tiene una particularidad y es que tiene mas objetos dentro de si. Esa particularidad se llama anidamiento, en ingles **NESTING.** 

Nesting: no solo tiene que ver con objetos, si no tambien con bloques de código. 

Anidamiento es un nivel de profundidad que tenemos de un contexto mas grande hacia uno mas pequeño.

![Untitled](JAVASCRIPT%2067342/Untitled%2031.png)

![Untitled](JAVASCRIPT%2067342/Untitled%2032.png)

Diferencias entre let , var y const

- Una de las diferencias es el bloque de codigo en donde estas existen

![Untitled](JAVASCRIPT%2067342/Untitled%2033.png)

**var** nos permite hacer una doble declaración, no es como const y let.

Ejemplo de USOS

Si quiero ver el valor de x, seria posible mostrarlo porque forma parte del bloque principal, pero si quiero ver el valor de i no puedo.

![Untitled](JAVASCRIPT%2067342/Untitled%2034.png)

Sin embargo si cambio la el tipo de variable de i , de let a var si se podria

![Untitled](JAVASCRIPT%2067342/Untitled%2035.png)

si la cambio por const, no me dejaría.

![Untitled](JAVASCRIPT%2067342/Untitled%2036.png)

la variable **i** no esta al alcance del **SCOPE** de afuera. Por que esta en el interior.

**Const y let** : se mantienen garbage collector, limpia. Ya que la variable no se usara mas fuera del alcance que tiene.

SCOPE = alcance

var se convierte en una variable global.

Lo ideal es usar const y let.

---

---

## Funciones

Estructura:

```jsx
function nombre_funcion(param1, param2){
	const resultado = param1+ param2;
  return resultado;
}

nombre_funcion(1,2) //Call the function
```

![Untitled](JAVASCRIPT%2067342/Untitled%2037.png)

![Untitled](JAVASCRIPT%2067342/Untitled%2038.png)

![Untitled](JAVASCRIPT%2067342/Untitled%2039.png)

Para JS es indiferente si declaramos una variable mas en los parametros de la funcion y no lo usamos.

---

---

## Métodos e iteradores

Métodos:

Son funciones que pertenecen a objetos.

Ejemplo: Metodo para obtener los nombres de una persona.

```jsx
const persona = {
	nombre: 'Monique',
	apellido: 'Matamoros',
	id: 5,
	nombreCompleto : function(){
		return `${this.nombre} ${this.apellido}`
	}
}

//llamado de la funcion
persona.nombreCompleto()
```

![Untitled](JAVASCRIPT%2067342/Untitled%2040.png)

### Arrays

```jsx
const miArray = [1,2,3, 'hola', 28, {a:1}]

miArray
```

![Untitled](JAVASCRIPT%2067342/Untitled%2041.png)

El array es de tipo object, pero este object es iterable

![Untitled](JAVASCRIPT%2067342/Untitled%2042.png)

Creare una variable iterador donde guardare el array

```jsx
var iterador = miArray[Symbol.iterator]();
```

![Untitled](JAVASCRIPT%2067342/Untitled%2043.png)

para saber si podemos iterar algo, debemos de verificar si tenemos el symbol iterator.

![Untitled](JAVASCRIPT%2067342/Untitled%2044.png)

El iterador en JS ya viene implícito y eso es porque le motor que corre JS , esta hecho en C++. Desde C++ se esta creando ese iterador.

---

---

## Arrays, iterables y Array.length

Dentro de las propiedades de un Array esta **Length = Longitud**

![Untitled](JAVASCRIPT%2067342/Untitled%2045.png)

Los Arrays ya tienen métodos implícitos, uno de ellos es push

```jsx
miArray.push(10) //Agregar al array un elemento nuevo que le de
//El retorno del array push es el length
```

![Untitled](JAVASCRIPT%2067342/Untitled%2046.png)

# Array.prototype.length

La propiedad **`length`** de un objeto que es una instancia de tipo Array establece o devuelve la cantidad de elementos en esa matriz. El valor es un entero sin signo de 32 bits que siempre es numéricamente mayor que el índice más alto en la matriz.

```jsx
const clothing = ['shoes', 'shirts', 'socks', 'sweaters'];

console.log(clothing.length);
// expected output: 4
```

---