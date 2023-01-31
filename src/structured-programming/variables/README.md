# Variables

Una variable es un elemento de datos con nombre cuyo valor puede cambiar durante el curso de la ejecución de un programa.

```
# Ejemplo variables en Javascript
var name
let phone
const dni
```

<b>Dato</b>: En informática, los datos son representaciones simbólicas (vale decir: numéricas, alfabéticas, algorítmicas, etc.) de un determinado atributo o variable cualitativa o cuantitativa.

```
# Ejemplo en Javascript
var name = 'Moises'
let phone = '1111111'
const dni = '123456789'
```

----

## Tipos de datos

#### Datos Primitivos
Son los tipos de datos del lenguaje y que no representan objetos, son valores simples.

<b>byte:</b> Representa un tipo de dato de 8 bits con signo. De tal manera que puede almacenar los valores numéricos de -128 a 127 (ambos inclusive).

<b>short:</b> Representa un tipo de dato de 16 bits con signo. De esta manera almacena valores numéricos de -32.768 a 32.767.

<b>int:</b> Es un tipo de dato de 32 bits con signo para almacenar valores numéricos. Cuyo valor mínimo es -231 y el valor máximo 231-1.

<b>long</b> Es un tipo de dato de 64 bits con signo que almacena valores numéricos entre -263 a 263-1

<b>float:</b> Es un tipo dato para almacenar números en coma flotante con precisión simple de 32 bits.

<b>double:</b> Es un tipo de dato para almacenar números en coma flotante con doble precisión de 64 bits.

<b>boolean:</b> Sirve para definir tipos de datos booleanos. Es decir, aquellos que tienen un valor de true o false. Ocupa 1 bit de información.

<b>char</b> Es un tipo de datos que representa a un carácter Unicode sencillo de 16 bits.

#### Datos Complejos

Los tipos compuestos se derivan de uno o más datos primitivos. A las distintas maneras de formar o combinar estos datos se les conocen con el nombre de “Estructura de datos”. Al combinarlo podemos crear un nuevo tipo, por ejemplo:

"array-de-enteros" es distinto al tipo "entero".

<b>string:</b> Es una secuencia de caracteres usado para representar un texto.

```
# Ejemplo en Javascript
let frase = 'Mi cadena de caracteres'
```

<b>array:</b> Es una estructura de datos que permite almacenar una serie de datos localizados por índices y separados por comas.

```
# Ejemplo en Javascript
let frutas = ['Banana', 'Fresa', 'Manzana']

let posiciones = [0, 1, 2, 3]
```

----

## Asignación de valores

Asignarle un dato a una variable consiste en reemplazar el valor anterior o inicial de la variable con un valor nuevo. Una vez que se asigna un nuevo valor, el valor anterior es eliminado de la memoria y no es posible recuperarlo.

Ejemplos:

```
## Asignacion de valores

# Asignacion: Array de strings
let listaMercado = ['arroz', 'azucar', 'harina', 'cafe', 'sal', 'aceite', 'mantequilla']

# Reemplazando el valor de la variable listaMercado
listaMercado = ['arroz', 'harina', 'melon']
```
