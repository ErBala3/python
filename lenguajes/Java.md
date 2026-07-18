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

## 6. Arrays y listas

- Un array guarda varios valores del mismo tipo.
- Se define escribiendo el tipo seguido de `[]`.
- Se puede acceder a cada elemento con su índice numérico.

```java
int[] numeros = {1, 2, 3};
System.out.println(numeros[0]);
```

## 7. Funciones

- `method`: es una función dentro de una clase.
- Puede recibir parámetros y devolver un valor con `return`.
- Se invoca usando el nombre del método.
- En Java, `public` significa que el método o atributo es accesible desde cualquier clase.
- `private` limita el acceso solo a la clase donde está declarado.
- `protected` permite acceder desde la clase, subclases y clases del mismo paquete.
- `static` indica que el método o atributo pertenece a la clase, no a una instancia concreta.

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

## 9. Estructuras de control

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

## 10. Manejo de excepciones

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

## 11. Clases

- `class`: define una plantilla para crear objetos.
- Un objeto es una instancia concreta de una clase.
- El constructor inicializa el estado del objeto.
- `this` permite referirse al objeto actual desde dentro de la clase.
- `public` permite acceder desde cualquier parte del programa.
- `private` limita el acceso solo a la propia clase.
- `protected` permite el acceso a clases hijas y al mismo paquete.
- `extends` permite crear clases hijas con herencia.
- `super()` llama al constructor de la clase padre.
- `final` impide que una clase pueda heredar de ella o que un método pueda sobrescribirse.
- `abstract` define una clase o método que debe implementarse en una subclase.
- `@Override` indica que un método está sobrescribiendo uno de la clase padre.

```java
class Persona {
    private String nombre;
    protected int edad;

    public Persona(String nombre, int edad) {
        this.nombre = nombre;
        this.edad = edad;
    }

    public String getNombre() {
        return nombre;
    }

    public void presentarse() {
        System.out.println("Hola, soy " + nombre);
    }
}

class Estudiante extends Persona {
    private String curso;

    public Estudiante(String nombre, int edad, String curso) {
        super(nombre, edad);
        this.curso = curso;
    }

    @Override
    public void presentarse() {
        System.out.println("Hola, soy " + getNombre() + " y estudio " + curso);
    }
}

Persona persona = new Persona("Ana", 25);
Estudiante estudiante = new Estudiante("Luis", 20, "Java");
persona.presentarse();
estudiante.presentarse();
```

## 12. Paquetes y bibliotecas

- `import`: permite reutilizar clases ya definidas.
- Java incluye muchas bibliotecas estándar para tareas comunes.

```java
import java.util.ArrayList;

ArrayList<String> nombres = new ArrayList<>();
nombres.add("Ana");
System.out.println(nombres.get(0));
```

## 13. Ejercicios

Para practicar lo aprendido, puedes hacer varios ejercicios y retos de programación en la siguiente página:

[Roadmap de Retos de Programación | by MoureDev](https://retosdeprogramacion.com/roadmap)
