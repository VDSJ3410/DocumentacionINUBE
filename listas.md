---
description: >-
  Las listas (ArrayList) son colecciones dinámicas que pueden almacenar
  múltiples valores. Son más flexibles que los arrays porque su tamaño puede
  cambiar.
---

# Listas

Una **lista** es una colección de elementos ordenados que permite almacenar múltiples valores en una sola variable.

* A diferencia de un **array**, el tamaño de la lista puede crecer o reducirse dinámicamente.
* Permite acceder a los elementos mediante un índice, empezando en 0.
* Se pueden agregar, eliminar y recorrer elementos fácilmente.
* Son muy utilizadas cuando se necesita manejar datos que cambian constantemente (ejemplo: lista de nombres de usuarios conectados).
* Ejemplo con números:

```
import java.util.ArrayList;

ArrayList<Integer> numeros = new ArrayList<>();
numeros.add(10);
numeros.add(20);
numeros.add(30);

for(Integer n : numeros) {
    System.out.println(n);
}
```

* Ejemplo con cadenas:

```
ArrayList<String> nombres = new ArrayList<>();
nombres.add("Ana");
nombres.add("Luis");
nombres.add("Sofía");

for(String nombre : nombres) {
    System.out.println(nombre);
}
```

_Conclusión:_ Las listas son una herramienta flexible y muy usada en Java porque permiten manejar colecciones dinámicas de datos de forma ordenada y sencilla.
