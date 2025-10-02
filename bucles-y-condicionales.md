---
description: >-
  En Java, los bucles permiten repetir un bloque de código, y las condicionales
  permiten tomar decisiones en el flujo del programa.
---

# Bucles y Condicionales

#### Bucles

* **while** → ejecuta el bloque mientras la condición sea verdadera.

```
int i = 1;
while(i <= 5) {
    System.out.println("Número: " + i);
    i++;
}
```

* **do-while** → primero ejecuta el bloque, luego evalúa la condición (se ejecuta al menos una vez).

```
int j = 1;
do {
    System.out.println("Número: " + j);
    j++;
} while(j <= 5);
```

* **for** → útil cuando conocemos el número de repeticiones.

```
for(int k = 1; k <= 5; k++) {
    System.out.println("Número: " + k);
}
```

#### Condicionales

* **if** → ejecuta el bloque si la condición es verdadera.

```
int edad = 20;
if(edad >= 18) {
    System.out.println("Es mayor de edad");
}
```

* **if-else** → ejecuta un bloque si la condición es verdadera y otro si es falsa.

```
int edad = 16;
if(edad >= 18) {
    System.out.println("Es mayor de edad");
} else {
    System.out.println("Es menor de edad");
}
```

_Conclusión:_ Los bucles permiten automatizar tareas repetitivas y las condicionales ayudan a tomar decisiones, juntos forman la base de la lógica en cualquier programa.
