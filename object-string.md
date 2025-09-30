---
description: String hereda de Object.  Por eso, puedes usar métodos de Object en un String
---

# Object – String

### Object:

* Es la **clase padre de todas las clases** en Java.
* Si una clase no hereda explícitamente de otra, automáticamente hereda de `Object`.
* Métodos más importantes:
  * `toString()`: convierte un objeto a texto.
  * `equals()`: compara objetos.
  * `hashCode()`: devuelve un código único para el objeto.
  * `getClass()`: devuelve la clase del objeto.

#### Ejemplo:

```
Object obj = new Integer(50);
System.out.println(obj.toString());   // "50"
System.out.println(obj.getClass());   // class java.lang.Integer

```

### String:

* `String` es una **clase especial para manejar texto**.
* Es un **objeto inmutable**: no se puede modificar una vez creado.
  * Si concatenas o cambias un `String`, en realidad se crea uno nuevo en memoria.

#### Creación de Strings:

```
String s1 = "Hola";                 // literal
String s2 = new String("Hola");     // objeto explícito

```

### Métodos comunes de String:

* `length()` → devuelve longitud.
* `charAt(i)` → obtiene un carácter.
* `substring(i, j)` → corta parte de la cadena.
* `equals()` y `equalsIgnoreCase()` → comparan contenido.
* `compareTo()` → compara alfabéticamente.
* `toUpperCase()` y `toLowerCase()` → cambian mayúsculas/minúsculas.
* `trim()` → elimina espacios.
* `contains("txt")` → busca subcadenas.

#### Ejemplo:

```
String texto = "  Java es Genial  ";
System.out.println(texto.trim());       // "Java es Genial"
System.out.println(texto.toUpperCase()); // "  JAVA ES GENIAL  "
System.out.println(texto.contains("Java")); // true

```

### Relación entre Object y String:

`String` hereda de `Object`, así que puede usar sus métodos (`toString`, `equals`, etc.).

#### Ejemplo:

```
String saludo = "Hola";
Object obj = saludo;
System.out.println(obj.toString()); // "Hola"

```

