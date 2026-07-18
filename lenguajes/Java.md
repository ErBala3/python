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

## 5. Operadores

### Aritméticos

```java
int suma = 1 + 2;
int resta = 5 - 3;
int multiplicacion = 4 * 2;
int division = 10 / 2;
int modulo = 10 % 3;
```

### Comparación

```java
int a = 5;
int b = 8;
System.out.println(a == b);
System.out.println(a != b);
System.out.println(a > b);
System.out.println(a < b);
```

### Lógicos

```java
System.out.println(true && false);
System.out.println(true || false);
System.out.println(!true);
```

### Asignación

```java
int variable = 1;
variable += 1;
variable -= 1;
variable *= 2;
variable /= 2;
variable %= 2;
```

### BITS

```java
int a = 3;
int b = 1;
System.out.println(a & b);
System.out.println(a | b);
System.out.println(a ^ b);
System.out.println(~a);
System.out.println(a >> 1);
System.out.println(a << 1);
```

## 6. Estructuras de control

### Condicionales

```java
int edad = 18;

if (edad >= 18) {
    System.out.println("Eres mayor de edad");
} else {
    System.out.println("Eres menor de edad");
}
```

### Bucles

```java
for (int i = 0; i < 3; i++) {
    System.out.println(i);
}
```

```java
int contador = 0;
while (contador < 3) {
    System.out.println(contador);
    contador += 1;
}
```

## 7. Manejo de excepciones

```java
try {
    System.out.println(10 / 0);
} catch (Exception e) {
    System.out.println("Se ha producido un error");
} finally {
    System.out.println("Fin del bloque");
}
```

## 8. Ejercicios

Para practicar lo aprendido, puedes hacer varios ejercicios y retos de programación en la siguiente página:

[Roadmap de Retos de Programación | by MoureDev](https://retosdeprogramacion.com/roadmap)
