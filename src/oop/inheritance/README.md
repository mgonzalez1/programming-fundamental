# Herencia

La <b>herencia</b> es la capacidad de crear nuevas clases sobre otras existentes.

La principal ventaja de la herencia es la reutilización de código. Si quieres crear una clase ligeramente diferente a una ya existente, no hay necesidad de duplicar el código. En su lugar, extiendes la clase existente y colocas la funcionalidad adicional dentro de una subclase resultante que hereda los campos y métodos de la superclase.

----

## Herencia simple

En la herencia simple, una clase hereda únicamente de una clase. No debemos confundirnos con este concepto y pensar que hablamos de niveles de herencia. Aunque en mi sistema existan varios niveles de herencia, al establecer una herencia simple cada una de las clases hereda solo de una clase.

## Herencia múltiple

Es la capacidad de una subclase de heredar de múltiples superclases.

## Abstracción y clases abstractas

<b>Abstracción</b>: La mayoría de las veces, cuando creas un programa con POO, das forma a los objetos del programa con base a objetos del mundo real. Sin embargo, los objetos del programa no representan a los originales con una precisión del 100 % (y rara vez es necesario que lo hagan). En su lugar, tus objetos tan solo copian atributos y comportamientos de objetos reales en un contexto específico, ignorando el resto.

<b>Clases abstractas</b>: Una clase abstracta es una clase común que posee atributos y métodos, y tiene como mínimo un método abstracto, además puede contener métodos normales. Esta clase no puede ser instanciada, solo puede heredarse, o sea no se puede usar para crear un objeto.

## Interfaces

Una interfaz es un conjunto de métodos y propiedades que no tiene ninguna implementación. La implementación la va a hacer cada uno de los elementos que herede de la interfaz dependiendo de sus necesidades.

## Polimorfismo

El término polimorfismo tiene origen en las palabras poly (muchos) y morfo (formas), y aplicado a la programación hace referencia a que los objetos pueden tomar diferentes formas, significa que objetos de diferentes clases pueden ser accedidos utilizando el mismo interfaz, mostrando un comportamiento distinto (tomando diferentes formas) según cómo sean accedidos.

```
# Ejemplo en Java

class Animal{ 
    public Animal() {} 
}

class Perro extends Animal {
    public Perro() {}
}

class Gato extends Animal {
    public Gato() {}
}

Animal a = new Perro()
```

Estamos asignando a una variable Animal un objeto de la clase Perro. ¿Cómo es esto posible?

Pues ahí lo tienes, el polimorfismo es lo que nos permite usar ambas clases de forma indistinta, ya que soportan el mismo “interfaz”.
