---
description: >-
  En Java, los Wrapper Classes son clases que representan a los tipos primitivos
  como objetos.
---

# Wrapper

### Lista de primitivos y sus Wrappers:

* `byte` → `Byte`
* `short` → `Short`
* `int` → `Integer`
* `long` → `Long`
* `float` → `Float`
* `double` → `Double`
* `char` → `Character`
* `boolean` → `Boolean`

### ¿Por qué existen los Wrapper?

* Porque **las colecciones (ArrayList, HashMap, etc.) no aceptan primitivos**, solo objetos.
* Para **usar métodos** que ayuden a convertir, comparar y manipular datos.
* Para representar valores **nulos** (ej: `Integer x = null;`), lo que no es posible con un primitivo.

### Métodos útiles:

* `parseInt("123")` → convierte texto a número.
* `toString(45)` → convierte número a texto.
* `compareTo(otroValor)` → compara valores.

### Ejemplo:&#x20;

```
int numPrimitivo = 7;
Integer numWrapper = numPrimitivo; // autoboxing
int otro = numWrapper; // unboxingSystem.out.println(Integer.parseInt("100") + 50); // 150
System.out.println(Integer.parseInt("100") + 50); // 150
```
