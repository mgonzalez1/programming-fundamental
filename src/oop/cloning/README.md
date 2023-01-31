# Clonación

El proceso de hacer una copia exacta del objeto en lugar de solo la referencia es llamado clonar. En la mayoría de los lenguajes, el mismo lenguaje o alguna librería puede facilitar alguna forma de realizar la copia. 

Por ejemplo en Java, la clase Object contiene el método clone(), que copia el objeto y retorna una referencia al objeto copiado. Como el método está definido en la clase Object, todas las clases definidas en Java podrán brindar este método al programador (para que el método funcione correctamente en algunos casos se deberá sobreescribir).

```
# Ejemplo en Java

Object original = new Object();
Object copia = null;

copia = original.clone(); // duplica el objeto y asigna la nueva referencia a 'copia'
```