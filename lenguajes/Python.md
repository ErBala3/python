# Python para principiantes

[Volver a la selección](../README.md)

Este repositorio sirve como una guía breve de estudio para aprender los fundamentos de Python.

## Objetivo

Aprender los conceptos básicos de forma práctica, con ejemplos sencillos y ordenados como una nota de estudio.

## 1. Comentarios

- Los comentarios sirven para explicar partes del código sin que Python las ejecute.
- Para comentarios largos se usa triple comillas:

```python
"""
Este es un comentario
muy largo
"""
```

- Para comentarios de una sola línea se usa `#`:

```python
# Este es un comentario de una línea
```

## 2. Variables y constantes

- Una variable es un nombre que almacena un valor.
- En Python no hace falta indicar el tipo al crear una variable.

```python
variable = "valor"
variable = 10
```

- No existen constantes reales como en otros lenguajes, pero se suelen escribir en mayúsculas para indicar que no deberían cambiar.

```python
CONSTANTE = "valor"
```

## 3. Tipos de datos

- `int`: números enteros.
- `float`: números decimales.
- `bool`: valores booleanos (`True` o `False`).
- `str`: cadenas de texto.

```python
entero = 10
decimal = 3.14
booleano = True
texto = "Hola mundo"
```

## 4. Mostrar mensajes

- `print()` sirve para mostrar información en pantalla.
- El texto que se muestra debe ir entre comillas.

```python
print("Hola mundo")
```

- Para insertar variables dentro de una cadena se usa `f` y `{}`.

```python
numero = 2
print(f"1 + 1 = {1 + 1}")
```

- Para unir varias cadenas se usa `+`.

```python
print("Hola " + "mundo")
```

## 5. Arrays y listas

- `list`: permite guardar varios valores en una sola variable.
- Se crean con corchetes `[]`.
- `append()`: añade un elemento al final de la lista.

```python
numeros = [1, 2, 3]
numeros.append(4)
print(numeros)
```

## 6. Funciones

- `def`: permite agrupar instrucciones y reutilizarlas.
- `return`: devuelve un valor desde la función.
- Las funciones ayudan a organizar el código y evitar repeticiones.
- En Python no existen prefijos como `public`, `private` o `protected` para funciones, pero sí es común usar convenciones de nombres para indicar intención.
- Un guion bajo simple (`_nombre`) suele indicar que un atributo o método es de uso interno.
- Un doble guion bajo (`__nombre`) provoca name mangling, que lo hace más difícil de acceder desde fuera.

```python
def saludar(nombre):
    return f"Hola {nombre}"

print(saludar("Ana"))
```

## 7. Cadenas de texto

- `str`: sirve para almacenar texto.
- Se pueden concatenar y transformar con métodos.

```python
texto = "hola"
print(texto.upper())
print(texto + " mundo")
```

## 8. Operadores

### Numéricos

- `+`: suma dos valores.

```python
suma = 1 + 2
```

- `-`: resta dos valores.

```python
resta = 1 - 2
```

- `*`: multiplica dos valores.

```python
multiplicacion = 1 * 2
```

- `**`: eleva una variable a otra.

```python
exponente = 1 ** 2
```

- `/`: divide y devuelve decimales.

```python
division = 1 / 2
```

- `//`: divide y devuelve el resultado sin decimales.

```python
division_entera = 1 // 2
```

- `%`: devuelve el resto de una división.

```python
modulo = 1 % 2
```

### Comparación

- `==`: compara si dos variables son iguales.

```python
a = 5
b = 8
print(a == b)
```

- `!=`: compara si dos variables son diferentes.

```python
a = 5
b = 8
print(a != b)
```

- `>`: compara si una variable es mayor que otra.

```python
a = 5
b = 8
print(a > b)
```

- `<`: compara si una variable es menor que otra.

```python
a = 5
b = 8
print(a < b)
```

- `>=`: compara si una variable es mayor o igual que otra.

```python
a = 5
b = 8
print(a >= b)
```

- `<=`: compara si una variable es menor o igual que otra.

```python
a = 5
b = 8
print(a <= b)
```

### Lógicos

- `and`: comprueba que dos condiciones son correctas.

```python
a = 2
b = 3
c = 5
print(a + b == c and b + c == 8)
```

- `or`: comprueba que al menos una condición es correcta.

```python
a = 2
b = 3
c = 5
print(a + b == 4 or b + c == 8)
```

- `not`: devuelve lo contrario de una condición.

```python
print(not (2 + 3 == 5))
```

### Asignación

- `=`: asigna un valor.

```python
variable = 1
```

- `+=`: suma y asigna el resultado.

```python
variable = 1
variable += 1
```

- `-=`: resta y asigna el resultado.

```python
variable = 1
variable -= 1
```

- `*=`: multiplica y asigna el resultado.

```python
variable = 1
variable *= 2
```

- `**=`: eleva y asigna el resultado.

```python
variable = 1
variable **= 2
```

- `/=`: divide y asigna el resultado.

```python
variable = 1
variable /= 2
```

- `//=`: divide entera y asigna el resultado.

```python
variable = 1
variable //= 2
```

- `%=`: calcula el módulo y asigna el resultado.

```python
variable = 1
variable %= 2
```

### Identidad

- `is`: comprueba si dos variables ocupan el mismo espacio en memoria.

```python
a = [1, 2]
b = a
print(a is b)
```

- `is not`: comprueba si dos variables ocupan distinto espacio en memoria.

```python
a = [1, 2]
b = [1, 2]
print(a is not b)
```

### Pertenencia

- `in`: comprueba si una variable contiene otra variable.

```python
print('a' in 'avion')
```

- `not in`: comprueba si una variable no contiene otra variable.

```python
print('a' not in 'avion')
```

### BITS

- `&`: comprueba bit a bit si ambos son 1 y devuelve 1.

```python
a = 3
b = 1
print(a & b)
```

- `|`: comprueba bit a bit si al menos uno es 1.

```python
a = 3
b = 1
print(a | b)
```

- `^`: comprueba bit a bit si ambos son diferentes.

```python
a = 3
b = 1
print(a ^ b)
```

- `~`: cambia los valores bit a bit y muestra el resultado contrario.

```python
a = 3
print(~a)
```

- `>>`: desplaza los bits a la derecha y rellena con 0.

```python
a = 3
print(a >> 1)
```

- `<<`: desplaza los bits a la izquierda y rellena con 0.

```python
a = 3
print(a << 1)
```

## 10. Estructuras de control

### Condicionales

- `if`: ejecuta un bloque de código si la condición es verdadera.
- `else`: ejecuta otro bloque si la condición no se cumple.
- `elif`: permite añadir más condiciones intermedias.

```python
edad = 18

if edad >= 18:
    print("Eres mayor de edad")
else:
    print("Eres menor de edad")
```

```python
numero = 5

if numero > 0:
    print("Es positivo")
elif numero == 0:
    print("Es cero")
else:
    print("Es negativo")
```

### Bucles

- `for`: repite una acción un número fijo de veces.
- `while`: repite una acción mientras se cumpla una condición.

```python
for i in range(10):
    print(i)
```

```python
contador = 0

while contador <= 10:
    print(contador)
    contador += 1
```

## 11. Manejo de excepciones

- `try`: intenta ejecutar un bloque de código.
- `except`: ejecuta otro bloque si ocurre un error.
- `finally`: se ejecuta siempre, haya o no error.

```python
try:
    print(10 / 0)
except:
    print("Se ha producido un error")
finally:
    print("Ha finalizado el manejo de excepciones")
```

## 12. Clases

- `class`: permite definir una plantilla para crear objetos.
- Un objeto es una instancia concreta de una clase.
- El método `__init__()` sirve para inicializar los valores del objeto.
- `self`: hace referencia al objeto actual y permite acceder a sus atributos y métodos.
- En Python, los atributos públicos se escriben normalmente sin guion bajo.
- Los atributos protegidos se suelen nombrar con un solo guion bajo (`_atributo`) para indicar que deberían usarse con cuidado.
- Los atributos privados se suelen nombrar con `__` para indicar que no deberían usarse desde fuera.
- La herencia permite crear clases nuevas a partir de otras usando `class Hija(Padre):`.
- `super()` permite reutilizar el constructor o métodos de la clase padre.
- Python no usa `public`, `private` o `protected` como palabras reservadas, pero sí tiene convenciones y mecanismos de encapsulación.
- Un método o atributo con un solo guion bajo se considera “protegido” por convención.
- Un método o atributo con doble guion bajo se convierte en privado por name mangling.

```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self._edad = edad

    def presentarse(self):
        return f"Hola, soy {self.nombre}"

    def get_edad(self):
        return self._edad

class Estudiante(Persona):
    def __init__(self, nombre, edad, curso):
        super().__init__(nombre, edad)
        self.curso = curso

    def presentarse(self):
        return f"Hola, soy {self.nombre} y estudio {self.curso}"

p = Persona("Ana", 25)
e = Estudiante("Luis", 20, "Python")
print(p.presentarse())
print(e.presentarse())
print(e.get_edad())
```

## 13. Módulos

- `import`: permite reutilizar funciones de otras bibliotecas.
- Python incluye muchos módulos útiles de forma estándar.

```python
import math
print(math.sqrt(16))
```

## 14. Ejercicios

Para practicar lo aprendido, puedes hacer varios ejercicios y retos de programación en la siguiente página:

[Roadmap de Retos de Programación | by MoureDev](https://retosdeprogramacion.com/roadmap)

Es una buena forma de reforzar conceptos como variables, condicionales, bucles, funciones y estructuras de datos.
