# Funciones

Las funciones, también llamados métodos, nos permiten dividir el trabajo que hace un programa, en tareas más pequeñas separadas de la parte principal. Ese es el concepto de función en programación.

Para definir una función, la sintaxis de las declaración es la siguiente:

```
[Modificadores] [function] [tipo_retorno] nombre_funcion ([argumentos])
{
    bloque_código;
}

# Ejemplos

# A)
function int suma(int num1, int num2)
{
    return num1 + num2;
}

# B)
public function int suma(int num1, int num2)
{
    return num1 + num2;
}

# C)
function suma(num1, num2)
{
    return num1 + num2;
}
```

Los *modificadores* pueden ser public, private, protected, virtual, static. Estos se usan cuando la funcion hace parte de una clase.

La palabra clave *function* identifica el bloque de sentencias de una función definida por el usuario.

El *tipo_retorno* puede ser un tipo de dato simple o compuesto

Los *argumentos* de una función, también llamados parámetros, representa una lista de variables cuyos valores son pasados al método para ser usados por éste. Suelen ser opcionales, por eso en el ejemplo están en corchetes []. Algunos métodos no aceptan argumentos.

El *bloque_codigo* es el código del método es la secuencia de instrucciones o sentencias que la función realiza.

```
# Funcion en Javascript 
function suma(num1, num2)
{
    return num1 + num2;
}

# Llamado de una funcion
let resultado = suma(5, 3);
console.log(resultado);


```

Dependiendo del lenguaje de programación, los modificadores, la palabra clave function, el tipo de valor retornado y el tipo de parametros de la funcion puede ser o no necesarios.

----

## Recursividad

La recursividad es una técnica muy empleada en la programación informática y consiste en que una función se llame a sí misma. 

El ejemplo clásico es la función que calcula el factorial de un número. Un factorial consiste en multiplicar un número natural por el número anterior, y este a su vez por el anterior, y así sucesivamente hasta llegar al número 1. Por ejemplo, el factorial de 8 sería el resultado de multiplicar 8 por 7, luego por 6 y así sucesivamente hasta llegar a uno.

```
# Ejemplo en Javascript

function factorial(numero) {
	// Sacar valor absoluto
	numero = Math.abs(numero);
	if (numero <= 1) return 1;
	return numero * factorial(numero - 1);
};

for (let x = 0; x < 10; x++) {
	console.log(`El factorial de ${x} es ${factorial(x)}`);
}
```

## Paso de variables por copia

Cuando es por valor o copia, la información de la variable se almacenan en una dirección de memoria diferente al recibirla en la funcion, por lo tanto si el valor de esa variable cambia no afecta la variable original, solo se modifica dentro del contexto de la función.

```
# Ejemplo en python

def doblar_valor(numero):
    numero *= 2

n = 10
doblar_valor(n)
print(n)
```

Los tipos de datos simples se pasan por valor: Enteros, flotantes, cadenas, lógicos...

## Paso de variables por referencia
Cuando es por referencia, la variable que se recibe como parámetro en la función apunta exactamente a la misma dirección de memoria que la variable original por lo que si dentro de la función se modifica su valor también se modifica la variable original.

```
# Ejemplo en python

def doblar_valores(numeros):
    for i,n in enumerate(numeros):
        numeros[i] *= 2

ns = [10,50,100]
doblar_valores(ns)
print(ns)
```

Los tipos de datos compuestos se pasan por referencia: Listas, diccionarios, conjuntos...


#### Diferencias entre paso de variables por copia y por referencia

La esencia de la diferencia corresponde a la libertad (o restricción) que existe sobre el parámetro de la función o método.

El paso por valor o copia se refiere a que se pasa una copia del valor del parámetro desde la función/método cliente. Al ser una copia, los cambios realizados directamente en la función/método sobre el valor del parámetro no serán reflejados al terminar la ejecución de la función/método.

El paso por referencia se refiere a que se pasa el mismo valor del parámetro desde la función/método cliente. Al ser el mismo valor, los cambios realizados directamente en la función/método sobre el valor del parámetro serán reflejados al terminar la ejecución de la función/método.

![](https://i.stack.imgur.com/8XAQ1.gif)
