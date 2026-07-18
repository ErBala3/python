# Python para principiantes

Este repositorio está pensado como una guía sencilla para aprender los fundamentos de Python desde cero. Aquí encontrarás ejemplos básicos de sintaxis, variables, tipos de datos, operadores, estructuras de control y manejo de excepciones.

## Objetivo

Aprender los conceptos básicos de Python de forma práctica y didáctica.

## 1. Comentarios

Los comentarios sirven para explicar partes del código.

```python
"""Este es un comentario de varias líneas"""
# Este es un comentario de una línea
```

## 2. Variables

En Python no hace falta declarar el tipo de una variable explícitamente.

```python
nombre = "Ana"
edad = 25
precio = 19.99
activo = True
```

## 3. Tipos de datos básicos

- `int`: números enteros
- `float`: números decimales
- `bool`: valores booleanos (`True` o `False`)
- `str`: cadenas de texto

```python
entero = 10
decimal = 3.14
booleano = True
texto = "Hola mundo"
```

## 4. Mostrar mensajes por pantalla

Para mostrar información en la consola se usa `print()`.

```python
print("Hola mundo")
```

También se puede insertar variables dentro de una cadena usando `f-strings`.

```python
nombre = "Luis"
print(f"Hola, {nombre}")
```

## 5. Operadores

### Aritméticos

```python
suma = 1 + 2
resta = 5 - 3
multiplicacion = 4 * 2
exponente = 2 ** 3
division = 10 / 2
division_entera = 10 // 3
modulo = 10 % 3
```

### Comparación

```python
a = 5
b = 8

print(a == b)  # Igualdad
print(a != b)  # Desigualdad
print(a > b)   # Mayor que
print(a < b)   # Menor que
print(a >= b)  # Mayor o igual
print(a <= b)  # Menor o igual
```

### Lógicos

```python
print(True and False)
print(True or False)
print(not True)
```

### Asignación

```python
valor = 1
valor += 1
valor -= 1
valor *= 2
valor /= 2
valor //= 2
valor %= 2
```

## 6. Estructuras de control

### Condicionales

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

#### `for`

```python
for i in range(5):
    print(i)
```

#### `while`

```python
contador = 0

while contador < 3:
    print(contador)
    contador += 1
```

## 7. Manejo de excepciones

```python
try:
    resultado = 10 / 0
except ZeroDivisionError:
    print("No se puede dividir entre cero")
finally:
    print("Fin del bloque")
```

## 8. Consejos para aprender

1. Practica cada día con pequeños ejercicios.
2. Lee los errores que aparecen en la consola.
3. Escribe tus propios ejemplos.
4. Divide los problemas en partes más pequeñas.

## 9. Siguiente paso

Para empezar a practicar, crea un archivo llamado `main.py` y prueba el siguiente ejemplo:

```python
print("¡Estoy aprendiendo Python!")
```

Luego ejecútalo con:

```bash
python main.py
```

## 10. Resumen rápido

Python es un lenguaje fácil de leer, muy usado en desarrollo web, automatización, ciencia de datos e inteligencia artificial. Con esta guía básica podrás empezar a familiarizarte con su sintaxis y sus conceptos fundamentales.

