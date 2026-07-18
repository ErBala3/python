# Python para principiantes

Este repositorio está pensado como una guía sencilla para aprender los fundamentos de Python desde cero. Aquí encontrarás ejemplos básicos de sintaxis, variables, tipos de datos, operadores, estructuras de control y manejo de excepciones.

## Objetivo

Aprender los conceptos básicos de Python de forma práctica y didáctica.

## 1. Comentarios

Para hacer comentarios grandes se usa triple comillas: `"""` o `'''`.

```python
"""
Este es un comentario
de varias líneas
"""
```

Para comentar una sola línea se usa `#`.

```python
# Este es un comentario de una línea
```

## 2. Variables y constantes

En Python no hace falta declarar el tipo de una variable explícitamente.

```python
variable = "valor"
variable = 10
```

No existen constantes en el sentido estricto, pero se suelen representar con letras mayúsculas.

```python
CONSTANTE = "valor"
```

## 3. Tipos de datos básicos

Hay cuatro tipos básicos de datos:

- `int`: números enteros
- `float`: números decimales
- `bool`: valores booleanos (`True` o `False`)
- `str`: cadenas de texto con comillas `""` o `''`

```python
entero = 10
decimal = 3.14
booleano = True
texto = "Hola mundo"
```

## 4. Mostrar mensajes por pantalla

Para imprimir información en pantalla se usa `print()` y el mensaje debe ir entre comillas.

```python
print("Hola mundo")
```

Para incluir variables dentro de una cadena se usa `f` delante de la cadena y se escriben las variables entre llaves `{}`.

```python
numero = 2
print(f"1 + 1 = {1 + 1}")
```

También se pueden concatenar cadenas con `+`.

```python
print("Hola " + "mundo")
```

## 5. Operadores

### Operadores numéricos

Cada uno se explica por separado, como en el archivo de teoría.

```python
suma = 1 + 2
```

```python
resta = 1 - 2
```

```python
multiplicacion = 1 * 2
```

```python
exponente = 1 ** 2
```

```python
division = 1 / 2
```

```python
division_entera = 1 // 2
```

```python
modulo = 1 % 2
```

### Operadores de comparación

```python
a = 5
b = 8
print(a == b)
```

```python
a = 5
b = 8
print(a != b)
```

```python
a = 5
b = 8
print(a > b)
```

```python
a = 5
b = 8
print(a < b)
```

```python
a = 5
b = 8
print(a >= b)
```

```python
a = 5
b = 8
print(a <= b)
```

### Operadores lógicos

```python
print(True and False)
```

```python
print(True or False)
```

```python
print(not True)
```

### Operadores de asignación

```python
variable = 1
```

```python
variable += 1
```

```python
variable -= 1
```

```python
variable *= 1
```

```python
variable **= 1
```

```python
variable /= 1
```

```python
variable //= 1
```

```python
variable %= 1
```

### Operadores de identidad

```python
a = [1, 2]
b = [1, 2]
print(a is b)
```

```python
a = [1, 2]
b = [1, 2]
print(a is not b)
```

### Operadores de pertenencia

```python
print('a' in 'avion')
```

```python
print('a' not in 'avion')
```

### Operadores a nivel de bits

```python
a = 3
b = 1
print(a & b)
```

```python
a = 3
b = 1
print(a | b)
```

```python
a = 3
b = 1
print(a ^ b)
```

```python
a = 3
print(~a)
```

```python
a = 3
print(a >> 1)
```

```python
a = 3
print(a << 1)
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
for i in range(10):
    print(i)
```

#### `while`

```python
contador = 0

while contador <= 10:
    print(contador)
    contador += 1
```

## 7. Manejo de excepciones

```python
try:
    print(10 / 0)
except:
    print("Se ha producido un error")
finally:
    print("Ha finalizado el manejo de excepciones")
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
