# Estructuras de control

Las estructuras de control son el conjunto de reglas que permiten controlar el flujo de ejecución de las instrucciones de un algoritmo o de un programa.

Las estructuras de control nos dan el poder de alterar, controlar o modificar el orden o el flujo en el que se ejecutan las instrucciones de un software a voluntad.

----

## Condicionales

Las condicionales son grupos de sentencias o sentencias individuales que te permiten condicionar la decisión entre la elección de una opción y otra. Un ejemplo de una condición en un lenguaje natural puede ser: si utilizas Python, puedes [o no] utilizar JavaScript. Las condicionales en programación, así como en el lenguaje natural, necesitan operadores lógicos, tales como if (que representa el si) o else (que puede representar un entonces).

#### If

<b>*If*</b> es un operador lógico con el que te encontrarás en un programa de código que cuente con condicionales. Este operador abre la condición y desencadena el poder de las condiciones que allí se van a desarrollar.

<b>*Else*</b> es otro operador lógico que representa la otra parte de la condición, es decir, el caso contrario que se ha establecido con el operador if. Aquí se construirá un flujo de ruta que se cumplirá cuando la condición sea falsa.

```
# Ejemplo en Javascript

if (edad >= 18) {
    console.log('Eres mayor de edad')
} else {
    console.log('Eres menor de edad')
}


if (edad >= 60) {
    console.log('Haces parte de la era edad')
} else if (edad >= 18) {
    console.log('Eres mayor de edad')
} else {
    console.log('Eres menor de edad')
}
```

#### Switch / case
Podemos tener la situación en que el flujo del programa puede depender de diversas opciones para continuar por un camino u otro. Podemos resolver esto empleando varios ‘else if‘, tantos como opciones tengamos, pero hay una instrucción algo más concisa para conseguir el mismo resultado según esta notación general: Switch case

La declaración <b>*switch*</b> evalúa una expresión, comparando el valor de esa expresión con una instancia case, y ejecuta declaraciones asociadas a ese case, así como las declaraciones en los case que siguen.

La palabra <b>*case*</b> indica el valor que va a verificar. Lo habitual es que sea un valor numérico o un texto. La combinación de la palabra case y su valor se llama etiqueta case.

La palabra clave <b>*default*</b> indica el bloque de código si no satisface ninguna de las etiquetas case que hemos escrito. Podemos decir que esta etiqueta es parecida a la sentencia else. También es una etiqueta opcional.

```
# Ejemplo en Javascript

switch (expr) {
  case 'Naranjas':
    console.log('El kilogramo de naranjas cuesta $0.59.');
    break;
  case 'Manzanas':
    console.log('El kilogramo de manzanas cuesta $0.32.');
    break;
  case 'Platanos':
    console.log('El kilogramo de platanos cuesta $0.48.');
    break;
  case 'Cerezas':
    console.log('El kilogramo de cerezas cuesta $3.00.');
    break;
  case 'Mangos':
  case 'Papayas':
    console.log('El kilogramo de mangos y papayas cuesta $2.79.');
    break;
  default:
    console.log('Lo lamentamos, por el momento no disponemos de ' + expr + '.');
}

console.log("¿Hay algo más que quisieras consultar?");
```

#### Diferencia y similitudes entre if y switch

El switch evalúa valores mientras que el if evalúa condiciones.

----

## Ciclos

Los bucles o ciclos de programación se utilizan en los programas de código para establecer sentencias o trozos de código que se repiten o se iteran.

#### For
Se usa cuando queremos repetir un conjunto de instrucciones un número finito de veces.

```
for (i = 0; i < total; i++)
{
    instrucciones;
}
```

#### While
Un bucle while itera o repite un bloque de código mientras una condición tiene el valor true

```
while (condicion)
{
    instrucciones;
}
```

La *condicion* que se evalúa a true o false, y se hace en cada repetición/iteración del bucle.

La *instruccion* o instrucciones que representa las líneas de código se ejecutan si la condicion es true.

#### Do While
Con la sentencia do while nos aseguramos a que las instrucciones se ejecuten una vez como mínimo. ¿Qué quiere decir esto?

Pues que ejecutamos primero todo el bloque de instrucciones, y al final siempre comprobaremos la condición para salir.

Dependiendo del lenguaje de programación, se puede escribir así:

```
do
{
    instrucciones;
} while (condicion);
```

#### Palabra clave “break”

Representa un alto completo en un bucle o sentencia switch. Es decir, cuando el programa se encuentra con esta palabra, interpreta que debe detener el bucle actual o si esta dentro de una sentencia switch la finaliza y no sigue comparando los demas *case*. Esta palabra se usa normalmente junto al condicional if. Entonces, podemos definir que si una variable llega a ser determinado valor, el bucle se detiene.

```
# Ejemplo en Javascript

let i = 0;

while (i < 6) {
  if (i === 3) {
    break;
  }
  i = i + 1;
}

console.log(i);
```