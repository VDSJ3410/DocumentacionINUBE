---
description: >-
  La Programación Orientada a Objetos (POO) es un paradigma que organiza el
  código en torno a objetos. Un objeto combina datos (atributos) y
  funcionalidades (métodos), lo que permite trabajar de manera.
---

# POO

Mientras la programación estructurada se centra en funciones y procedimientos, la POO se centra en **modelar entidades** y sus comportamientos.

### Conceptos Fundamentales:

#### 🔹 Clase

* Es el **molde o plantilla** que define cómo serán los objetos.
* Contiene atributos (propiedades) y métodos (acciones).

Ejemplo:

```
class Coche {
    String color;
    int velocidad;
    
    void acelerar() {
        velocidad += 10;
    }
}
```

#### 🔹 Objeto

* Es una **instancia concreta de una clase**.
* Cada objeto tiene sus propios valores en los atributos, aunque comparten la misma estructura de la clase.

```
Coche miCoche = new Coche();
miCoche.color = "Rojo";
miCoche.acelerar();
```

#### 🔹 Atributos

* Son las **características** de un objeto.\
  Ejemplo: color, tamaño, nombre, edad.

#### 🔹 Métodos

* Son las **acciones o comportamientos** de un objeto.\
  Ejemplo: acelerar(), dormir(), encender().

### Principios de la POO:

#### 1. **Encapsulamiento**

* Consiste en proteger los datos del objeto y exponer solo lo necesario.
* Se logra con modificadores de acceso (`private`, `public`, `protected`).

```
class Persona {
    private String nombre;

    public void setNombre(String n) {
        nombre = n;
    }

    public String getNombre() {
        return nombre;
    }
}
```

#### 2. **Herencia**

* Permite crear nuevas clases a partir de otras ya existentes.
* Favorece la **reutilización de código**.

```
class Animal {
    void comer() {
        System.out.println("El animal come.");
    }
}

class Perro extends Animal {
    void ladrar() {
        System.out.println("Guau!");
    }
}
```

#### 3. **Polimorfismo**

* Un mismo método puede comportarse de **formas distintas** dependiendo del objeto.

Ejemplo con sobreescritura:

```
class Animal {
    void sonido() {
        System.out.println("Sonido genérico");
    }
}

class Gato extends Animal {
    @Override
    void sonido() {
        System.out.println("Miau");
    }
}
```

#### 4. **Abstracción**

* Permite centrarse en lo **importante** de un objeto, ocultando lo irrelevante.
* Se logra con **clases abstractas** e **interfaces**.

```
abstract class Figura {
    abstract void dibujar();
}
```

### 4. Beneficios de la POO

✅ Código más organizado y legible.\
✅ Facilita la reutilización de componentes.\
✅ Permite mantener y escalar proyectos grandes.\
✅ Se asemeja al mundo real, haciendo más natural la programación.
