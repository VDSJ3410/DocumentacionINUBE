---
description: >-
  Un Map guarda pares clave-valor. Cada clave es única y se asocia a un valor.
  El más común es HashMap.
---

# Mapas

Un **mapa** es una estructura que guarda **pares clave-valor**.

* Cada clave es única y permite acceder a su valor asociado.
* Es muy útil para búsquedas rápidas: en lugar de recorrer toda una lista, se accede directamente usando la clave.
* Ejemplos de uso:
  * Guardar usuarios por su ID.
  * Relacionar matrículas con alumnos.
  * Relacionar ISBN con libros.
* Los mapas facilitan la organización de datos cuando se necesita asociar información de manera directa.
* Ejemplo básico:

```
import java.util.HashMap;

HashMap<String, String> paises = new HashMap<>();
paises.put("MX", "México");
paises.put("US", "Estados Unidos");
paises.put("ES", "España");

System.out.println(paises.get("MX")); // México
```

* Recorrer un mapa:

```
for(String clave : paises.keySet()) {
    System.out.println(clave + " -> " + paises.get(clave));
}
```

_Conclusión:_ Los mapas destacan por su rapidez al buscar y relacionar información mediante claves, siendo una estructura ideal para proyectos que requieren eficiencia en el acceso a datos.
