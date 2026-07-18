# Java para principiantes

[Volver a la selección](../README.md)

Este documento presenta una guía breve de estudio para aprender los fundamentos de Java.

## Objetivo

Aprender los conceptos básicos de forma práctica, con ejemplos sencillos y adaptados a Java.

## 1. Comentarios

- Los comentarios sirven para explicar partes del código sin que Java las ejecute.
- Para comentarios de una línea se usa `//`:

```java
// Esto es un comentario de una línea
```

- Para comentarios largos se usa `/* ... */`:

```java
/*
Esto es un comentario
multilínea
*/
```

## 2. Variables y constantes

- En Java se debe indicar el tipo de variable.
- `final` se usa para valores que no cambian.

```java
String nombre = "Ana";
int edad = 25;
final double PI = 3.1416;
```

## 3. Tipos de datos

- `int`: enteros.
- `double`: números decimales.
- `boolean`: valores `true` o `false`.
- `String`: texto.

```java
int entero = 10;
double decimal = 3.14;
boolean activo = true;
String texto = "Hola mundo";
```

## 4. Mostrar mensajes

- `System.out.println()` sirve para mostrar información en consola.

```java
System.out.println("Hola mundo");
```

## 5. Arrays y listas

- Un array guarda varios valores del mismo tipo.
- Se define escribiendo el tipo seguido de `[]`.

```java
int[] numeros = {1, 2, 3};
System.out.println(numeros[0]);
```

## 6. Objetos

- `class`: define un tipo con propiedades y métodos.
- Un objeto se crea con `new`.

```java
class Persona {
    String nombre;
    int edad;
}

Persona persona = new Persona();
persona.nombre = "Ana";
persona.edad = 25;
System.out.println(persona.nombre);
```

## 7. Funciones

- `method`: es una función dentro de una clase.
- Se invoca usando el nombre del método.

```java
class Ejemplo {
    static String saludar(String nombre) {
        return "Hola " + nombre;
    }
}

System.out.println(Ejemplo.saludar("Ana"));
```

## 8. Cadenas de texto

- `String`: sirve para almacenar texto.
- Se pueden comparar, concatenar y transformar con métodos.

```java
String texto = "hola";
System.out.println(texto.toUpperCase());
```

## 9. Entrada de datos

- `Scanner`: permite leer datos introducidos por el usuario.
- Se usa para capturar texto o números desde consola.

```java
import java.util.Scanner;

Scanner scanner = new Scanner(System.in);
String nombre = scanner.nextLine();
System.out.println("Hola " + nombre);
```

## 10. Operadores

### Numéricos

- `+`: suma dos valores.

```java
int suma = 1 + 2;
```

- `-`: resta dos valores.

```java
int resta = 1 - 2;
```

- `*`: multiplica dos valores.

```java
int multiplicacion = 1 * 2;
```

- `Math.pow()`: eleva un valor a una potencia.

```java
double exponente = Math.pow(2, 3);
System.out.println(exponente);
```

- `/`: divide y devuelve decimales.

```java
double division = 1 / 2.0;
```

- `%`: devuelve el resto de una división.

```java
int modulo = 1 % 2;
```

### Comparación

- `==`: compara si dos variables son iguales.

```java
int a = 5;
int b = 8;
System.out.println(a == b);
```

- `!=`: compara si dos variables son diferentes.

```java
int a = 5;
int b = 8;
System.out.println(a != b);
```

- `>`: compara si una variable es mayor que otra.

```java
int a = 5;
int b = 8;
System.out.println(a > b);
```

- `<`: compara si una variable es menor que otra.

```java
int a = 5;
int b = 8;
System.out.println(a < b);
```

- `>=`: compara si una variable es mayor o igual que otra.

```java
int a = 5;
int b = 8;
System.out.println(a >= b);
```

- `<=`: compara si una variable es menor o igual que otra.

```java
int a = 5;
int b = 8;
System.out.println(a <= b);
```

### Lógicos

- `&&`: comprueba que dos condiciones son correctas.

```java
System.out.println(true && false);
```

- `||`: comprueba que al menos una condición es correcta.

```java
System.out.println(true || false);
```

- `!`: devuelve lo contrario de una condición.

```java
System.out.println(!true);
```

### Asignación

- `=`: asigna un valor.

```java
int variable = 1;
```

- `+=`: suma y asigna el resultado.

```java
int variable = 1;
variable += 1;
```

- `-=`: resta y asigna el resultado.

```java
int variable = 1;
variable -= 1;
```

- `*=`: multiplica y asigna el resultado.

```java
int variable = 1;
variable *= 2;
```

- `/=`: divide y asigna el resultado.

```java
int variable = 1;
variable /= 2;
```

- `%=`: calcula el módulo y asigna el resultado.

```java
int variable = 1;
variable %= 2;
```

### BITS

- `&`: comprueba bit a bit si ambos son 1.

```java
int a = 3;
int b = 1;
System.out.println(a & b);
```

- `|`: comprueba bit a bit si al menos uno es 1.

```java
int a = 3;
int b = 1;
System.out.println(a | b);
```

- `^`: comprueba bit a bit si ambos son diferentes.

```java
int a = 3;
int b = 1;
System.out.println(a ^ b);
```

- `~`: cambia los valores bit a bit y muestra el resultado contrario.

```java
int a = 3;
System.out.println(~a);
```

- `>>`: desplaza los bits a la derecha y rellena con 0.

```java
int a = 3;
System.out.println(a >> 1);
```

- `<<`: desplaza los bits a la izquierda y rellena con 0.

```java
int a = 3;
System.out.println(a << 1);
```

## 11. Estructuras de control

### Condicionales

- `if`: ejecuta un bloque si la condición es verdadera.
- `else`: ejecuta otro bloque si la condición no se cumple.
- `else if`: añade más condiciones intermedias.

```java
int edad = 18;

if (edad >= 18) {
    System.out.println("Eres mayor de edad");
} else {
    System.out.println("Eres menor de edad");
}
```

```java
int numero = 5;

if (numero > 0) {
    System.out.println("Es positivo");
} else if (numero == 0) {
    System.out.println("Es cero");
} else {
    System.out.println("Es negativo");
}
```

### Bucles

- `for`: repite una acción un número fijo de veces.
- `while`: repite una acción mientras se cumpla una condición.

```java
for (int i = 0; i < 10; i++) {
    System.out.println(i);
}
```

```java
int contador = 0;
while (contador <= 10) {
    System.out.println(contador);
    contador += 1;
}
```

## 12. Manejo de excepciones

- `try`: intenta ejecutar un bloque de código.
- `catch`: ejecuta otro bloque si ocurre un error.
- `finally`: se ejecuta siempre, haya o no error.

```java
try {
    System.out.println(10 / 0);
} catch (Exception e) {
    System.out.println("Se ha producido un error");
} finally {
    System.out.println("Fin del bloque");
}
```

## 13. Clases

- `class`: define un tipo con propiedades y métodos.
- Se crean objetos con `new`.

```java
class Persona {
    String nombre;

    Persona(String nombre) {
        this.nombre = nombre;
    }
}

Persona persona = new Persona("Ana");
System.out.println(persona.nombre);
```

## 14. Paquetes y bibliotecas

- `import`: permite reutilizar clases ya definidas.
- Java incluye muchas bibliotecas estándar para tareas comunes.

```java
import java.util.ArrayList;

ArrayList<String> nombres = new ArrayList<>();
nombres.add("Ana");
System.out.println(nombres.get(0));
```

## 15. Ejercicios

Para practicar lo aprendido, puedes hacer varios ejercicios y retos de programación en la siguiente página:

[Roadmap de Retos de Programación | by MoureDev](https://retosdeprogramacion.com/roadmap)
