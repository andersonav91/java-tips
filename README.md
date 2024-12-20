# Java tips
Lista de tips y contenido útil para java.

-----------

### Variables Primitivas en Java

En Java, las variables primitivas son los tipos de datos más básicos que se utilizan para almacenar valores simples. Hay **8 tipos de datos primitivos** en Java.

| Tipo     | Tamaño (bits) | Valor Mínimo                  | Valor Máximo                  | Ejemplo               |
|----------|---------------|-------------------------------|-------------------------------|-----------------------|
| `byte`   | 8             | -128                          | 127                           | `byte edad = 25;`     |
| `short`  | 16            | -32,768                       | 32,767                        | `short valor = 1234;` |
| `int`    | 32            | -2,147,483,648                | 2,147,483,647                 | `int num = 1000;`     |
| `long`   | 64            | -9,223,372,036,854,775,808    | 9,223,372,036,854,775,807     | `long l = 12345L;`    |
| `float`  | 32            | ±1.4E-45                      | ±3.4E+38                      | `float f = 1.5f;`     |
| `double` | 64            | ±4.9E-324                     | ±1.8E+308                     | `double d = 3.14;`    |
| `char`   | 16            | '\u0000'                      | '\uffff'                      | `char c = 'A';`       |
| `boolean`| 1 (aprox.)    | `false`                       | `true`                        | `boolean b = true;`   |

**Notas**
- Los tipos primitivos son más eficientes en términos de uso de memoria y rendimiento.
- Para datos más complejos, se utilizan clases y objetos.
- Los datos primitivos no pueden tener valor null.

-----------

### Constantes en Java

En Java, las **constantes** son valores que no cambian durante la ejecución del programa. Se definen como variables cuyo contenido es inmutable una vez inicializado. Esto se logra utilizando la palabra clave `final`.

**Características de las Constantes** 
1. **Inmutables**: Una vez asignado un valor, no puede cambiar.
2. **Visibilidad**: Generalmente se definen como `static final` para que puedan ser accesibles sin instanciar una clase.
3. **Convención de Nombres**: Los nombres de las constantes suelen escribirse en mayúsculas, con palabras separadas por guiones bajos (`_`).

**Declaración de Constantes**

Para definir una constante en Java, se utiliza la palabra clave `final`. Opcionalmente, se combina con `static` si la constante es compartida por todas las instancias de la clase.

**Ejemplo de Constante**
```java
// Declaración de una constante
public static final double PI = 3.14159;
```
**Notas**
- Java no genera excepción si se intenta modificar una constante, pero si un error de compilación:

```java
error: cannot assign a value to final variable <nombre_constante>
```
-----------




