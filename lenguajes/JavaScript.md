# JavaScript para principiantes

[Volver a la selección](../README.md)

Este documento presenta una guía breve de estudio para aprender los fundamentos de JavaScript.

## Objetivo

Aprender los conceptos básicos de forma práctica, con ejemplos sencillos y adaptados a JavaScript.

## 1. Comentarios

- Los comentarios sirven para explicar partes del código sin que JavaScript las ejecute.
- Para comentarios de una línea se usa `//`:

```javascript
// Esto es un comentario de una línea
```

- Para comentarios largos se usa `/* ... */`:

```javascript
/*
Esto es un comentario
multilínea
*/
```

## 2. Variables

- `let` permite cambiar el valor de una variable.
- `const` sirve para valores que no deben cambiar.

```javascript
let nombre = "Ana";
const edad = 25;
```

## 3. Tipos de datos

- `string`: cadenas de texto.
- `number`: números.
- `boolean`: valores `true` o `false`.
- `object`: objetos.
- `array`: listas.

```javascript
let texto = "Hola";
let numero = 10;
let activo = true;
let persona = { nombre: "Ana" };
let lista = [1, 2, 3];
```

## 4. Mostrar mensajes

- `console.log()` sirve para mostrar información en la consola.

```javascript
console.log("Hola mundo");
```

## 5. Operadores

### Aritméticos

```javascript
let suma = 1 + 2;
let resta = 5 - 3;
let multiplicacion = 4 * 2;
let division = 10 / 2;
let modulo = 10 % 3;
```

### Comparación

- `==` compara valores de forma flexible.
- `===` compara valor y tipo de forma estricta.

```javascript
let a = 5;
let b = "5";
console.log(a == b);
console.log(a === b);
```

### Lógicos

```javascript
console.log(true && false);
console.log(true || false);
console.log(!true);
```

### Asignación

```javascript
let variable = 1;
variable += 1;
variable -= 1;
variable *= 2;
variable /= 2;
variable %= 2;
```

### Pertenencia

- `in` comprueba si una propiedad existe en un objeto.
- `instanceof` comprueba si un objeto es instancia de una clase.

```javascript
let persona = { nombre: "Ana" };
console.log("nombre" in persona);
```

### BITS

```javascript
let a = 3;
let b = 1;
console.log(a & b);
console.log(a | b);
console.log(a ^ b);
console.log(~a);
console.log(a >> 1);
console.log(a << 1);
```

## 6. Estructuras de control

### Condicionales

```javascript
let edad = 18;

if (edad >= 18) {
  console.log("Eres mayor de edad");
} else {
  console.log("Eres menor de edad");
}
```

### Bucles

```javascript
for (let i = 0; i < 3; i++) {
  console.log(i);
}
```

```javascript
let contador = 0;
while (contador < 3) {
  console.log(contador);
  contador += 1;
}
```

## 7. Manejo de excepciones

```javascript
try {
  console.log(10 / 0);
} catch (error) {
  console.log("Se ha producido un error");
} finally {
  console.log("Fin del bloque");
}
```

## 8. Ejercicios

Para practicar lo aprendido, puedes hacer varios ejercicios y retos de programación en la siguiente página:

[Roadmap de Retos de Programación | by MoureDev](https://retosdeprogramacion.com/roadmap)
