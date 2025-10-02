---
description: >-
  Una lista también puede almacenar objetos creados a partir de clases. Esto
  permite guardar datos más complejos.
---

# Listas con Objetos

Las listas también pueden contener **objetos completos**, no solo valores simples.

* Cada objeto puede tener varios atributos (ejemplo: nombre, edad, dirección).
* Esto hace que las listas sean más poderosas, porque permiten representar información del mundo real.
* Se pueden recorrer para mostrar atributos de cada objeto, modificarlos o buscar un elemento específico.
* Son comunes en proyectos donde se necesita manejar registros (ejemplo: lista de clientes, lista de libros en una biblioteca).
* Ejemplo:&#x20;

```
import java.util.ArrayList;

class Persona {
    String nombre;
    int edad;

    Persona(String nombre, int edad) {
        this.nombre = nombre;
        this.edad = edad;
    }
}

ArrayList<Persona> personas = new ArrayList<>();
personas.add(new Persona("Ana", 22));
personas.add(new Persona("Luis", 25));

for(Persona p : personas) {
    System.out.println(p.nombre + " - " + p.edad);
}
```

_Conclusión:_ Usar listas de objetos acerca la programación a la vida real, ya que cada elemento puede representar entidades completas con múltiples características.
