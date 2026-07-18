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

```python
a = 5
b = 8
print(a == b)
```

- Desigualdad `!=`:

```python
a = 5
b = 8
print(a != b)
```

- Mayor que `>`:

```python
a = 5
b = 8
print(a > b)
```

- Menor que `<`:

```python
a = 5
b = 8
print(a < b)
```

- Mayor o igual que `>=`:

```python
a = 5
b = 8
print(a >= b)
```

- Menor o igual que `<=`:

```python
a = 5
b = 8
print(a <= b)
```

### Lógicos

- `and`:

```python
print(True and False)
```

- `or`:

```python
print(True or False)
```

- `not`:

```python
print(not True)
```

### Asignación

- Asignar un valor `=`:

```python
variable = 1
```

- Sumar y asignar `+=`:

```python
variable = 1
variable += 1
```

- Restar y asignar `-=`:

```python
variable = 1
variable -= 1
```

- Multiplicar y asignar `*=`:

```python
variable = 1
variable *= 2
```

- Elevar y asignar `**=`:

```python
variable = 1
variable **= 2
```

- Dividir y asignar `/=`:

```python
variable = 1
variable /= 2
```

- Dividir entero y asignar `//=`:

```python
variable = 1
variable //= 2
```

- Sacar el módulo y asignar `%=`:

```python
variable = 1
variable %= 2
```

### Identidad

- `is`:

```python
a = [1, 2]
b = [1, 2]
print(a is b)
```

- `is not`:

```python
a = [1, 2]
b = [1, 2]
print(a is not b)
```

### Pertenencia

- `in`:

```python
print('a' in 'avion')
```

- `not in`:

```python
print('a' not in 'avion')
```

### BITS

- `&`:

```python
a = 3
b = 1
print(a & b)
```

- `|`:

```python
a = 3
b = 1
print(a | b)
```

- `^`:

```python
a = 3
b = 1
print(a ^ b)
```

- `~`:

```python
a = 3
print(~a)
```

- `>>`:

```python
a = 3
print(a >> 1)
```

- `<<`:

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
