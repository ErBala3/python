# Python para principiantes

Este repositorio sirve como una guía breve de estudio para aprender los fundamentos de Python.

## Objetivo

Aprender los conceptos básicos de forma práctica, con ejemplos sencillos y ordenados como una nota de estudio.

## 1. Comentarios

- Para comentarios largos se usa triple comillas:

```python
"""
comentario
"""
```

- Para comentarios de una sola línea se usa `#`:

```python
# comentario
```

## 2. Variables y constantes

- No hace falta indicar el tipo al crear una variable.

```python
variable = "valor"
variable = 10
```

- No existen constantes reales, pero se suelen escribir en mayúsculas.

```python
CONSTANTE = "valor"
```

## 3. Tipos de datos

- `int`: enteros
- `float`: decimales
- `bool`: booleanos (`True` / `False`)
- `str`: cadenas de texto

```python
entero = 10
decimal = 3.14
booleano = True
texto = "Hola mundo"
```

## 4. Mostrar mensajes

- Se usa `print()` para mostrar texto.

```python
print("Hola mundo")
```

- Para meter variables dentro de una cadena se usa `f` y `{}`.

```python
numero = 2
print(f"1 + 1 = {1 + 1}")
```

- Para unir cadenas se usa `+`.

```python
print("Hola " + "mundo")
```

## 5. Operadores

### Numéricos

- Suma `+`:

```python
suma = 1 + 2
```

- Resta `-`:

```python
resta = 1 - 2
```

- Multiplicación `*`:

```python
multiplicacion = 1 * 2
```

- Exponente `**`:

```python
exponente = 1 ** 2
```

- División `/`:

```python
division = 1 / 2
```

- División entera `//`:

```python
division_entera = 1 // 2
```

- Módulo `%`:

```python
modulo = 1 % 2
```

### Comparación

- Igualdad `==`:
  - Compara si dos variables son iguales.

```python
a = 5
b = 8
print(a == b)
```

- Desigualdad `!=`:
  - Compara si dos variables son diferentes.

```python
a = 5
b = 8
print(a != b)
```

- Mayor que `>`:
  - Compara si una variable es mayor que otra.

```python
a = 5
b = 8
print(a > b)
```

- Menor que `<`:
  - Compara si una variable es menor que otra.

```python
a = 5
b = 8
print(a < b)
```

- Mayor o igual que `>=`:
  - Compara si una variable es mayor o igual que otra.

```python
a = 5
b = 8
print(a >= b)
```

- Menor o igual que `<=`:
  - Compara si una variable es menor o igual que otra.

```python
a = 5
b = 8
print(a <= b)
```

### Lógicos

- `and`:
  - Comprueba que dos condiciones son correctas.

```python
a = 2
b = 3
c = 5
print(a + b == c and b + c == 8)
```

- `or`:
  - Comprueba que al menos una condición es correcta.

```python
a = 2
b = 3
c = 5
print(a + b == 4 or b + c == 8)
```

- `not`:
  - Comprueba si se cumple la condición y devuelve lo contrario.

```python
print(not (2 + 3 == 5))
```

### Asignación

- `=`:
  - Asigna un valor.

```python
variable = 1
```

- `+=`:
  - Sumar y asignar un valor.

```python
variable = 1
variable += 1
```

- `-=`:
  - Restar y asignar un valor.

```python
variable = 1
variable -= 1
```

- `*=`:
  - Multiplicar y asignar un valor.

```python
variable = 1
variable *= 2
```

- `**=`:
  - Elevar y asignar un valor.

```python
variable = 1
variable **= 2
```

- `/=`:
  - Dividir y asignar un valor.

```python
variable = 1
variable /= 2
```

- `//=`:
  - Dividir entero y asignar un valor.

```python
variable = 1
variable //= 2
```

- `%=`:
  - Sacar el módulo y asignar un valor.

```python
variable = 1
variable %= 2
```

### Identidad

- `is`:
  - Comprueba si dos variables ocupan el mismo espacio en memoria.

```python
a = [1, 2]
b = a
print(a is b)
```

- `is not`:
  - Comprueba si dos variables ocupan distinto espacio en memoria.

```python
a = [1, 2]
b = [1, 2]
print(a is not b)
```

### Pertenencia

- `in`:
  - Comprueba si una variable contiene otra variable.

```python
print('a' in 'avion')
```

- `not in`:
  - Comprueba si una variable no contiene otra variable.

```python
print('a' not in 'avion')
```

### BITS

- `&`:
  - Comprueba bit a bit si ambos son 1 y lo cambia por uno y da el resultado.

```python
a = 3
b = 1
print(a & b)
```

- `|`:
  - Comprueba bit a bit si al menos uno es 1 y lo cambia por uno y da el resultado.

```python
a = 3
b = 1
print(a | b)
```

- `^`:
  - Comprueba bit a bit si ambos son diferentes y lo cambia por uno y da el resultado.

```python
a = 3
b = 1
print(a ^ b)
```

- `~`:
  - Cambia los valores bit a bit y muestra el resultado.

```python
a = 3
print(~a)
```

- `>>`:
  - Desplaza los bits x números a la derecha y rellena lo demás con 0.

```python
a = 3
print(a >> 1)
```

- `<<`:
  - Desplaza los bits x números a la izquierda y rellena lo demás con 0.

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

- `for`:

```python
for i in range(10):
    print(i)
```

- `while`:

```python
contador = 0

while contador <= 10:
    print(contador)
    contador += 1
```

## 7. Manejo de excepciones

- `try`:
  - Intenta ejecutar código.

```python
try:
    print(10 / 0)
```

- `except`:
  - Si no se puede ejecutar el código, ejecuta otra línea de código.

```python
try:
    print(10 / 0)
except:
    print("Se ha producido un error")
```

- `finally`:
  - Se ejecuta siempre al finalizar el manejo de excepciones, haya o no errores.

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

Crea un archivo llamado `main.py` y prueba este ejemplo:

```python
print("¡Estoy aprendiendo Python!")
```

Ejecuta el archivo con:

```bash
python main.py
```

## 10. Resumen rápido

Python es un lenguaje simple y fácil de leer. Se usa mucho en desarrollo web, automatización, ciencia de datos e inteligencia artificial.
