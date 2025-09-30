---
description: >-
  Consejo: usa primitivos cuando necesites eficiencia y Wrappers cuando trabajes
  con colecciones o necesites métodos extra.
---

# Primitivos vs. Wrapper

{% tabs %}
{% tab title="Característica" %}
Tipo

Valor por defecto

Métodos disponibles

Uso en colecciones

Rendimiento
{% endtab %}

{% tab title="Primitivo (int, double)" %}
Dato simple

0, 0.0, false

Ninguno

No

Más rápido, menos memoria
{% endtab %}

{% tab title="Wrapper (Integer, Double)" %}
Objeto

null

Sí (ej: `toString()`, `compareTo()`)

Sí (`ArrayList<Integer>`)

Más lento, ocupa más memoria
{% endtab %}
{% endtabs %}

### Conceptos clave:

* **Autoboxing**: conversión automática de primitivo → Wrapper.
* **Unboxing**: conversión automática de Wrapper → primitivo.

#### Ejemplo práctico:

```
ArrayList<Integer> numeros = new ArrayList<>();
numeros.add(10);     // autoboxing: int → Integer
int valor = numeros.get(0); // unboxing: Integer → int

```

