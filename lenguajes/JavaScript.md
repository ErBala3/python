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

## 5. Arrays y listas

- `array`: permite guardar varios valores en una sola variable.
- Se crean con corchetes `[]`.

```javascript
let numeros = [1, 2, 3];
numeros.push(4);
console.log(numeros);
```

## 6. Objetos

- `object`: agrupa datos relacionados mediante pares clave-valor.
- Se define con llaves `{}`.

```javascript
let persona = { nombre: "Ana", edad: 25 };
console.log(persona.nombre);
```

## 7. Funciones

- `function`: permite encapsular una tarea y reutilizarla.
- También se pueden usar funciones flecha.

```javascript
function saludar(nombre) {
  return `Hola ${nombre}`;
}

console.log(saludar("Ana"));
```

## 8. Cadenas de texto

- `string`: sirve para almacenar texto.
- Se pueden modificar con métodos como `toUpperCase()`.

```javascript
let texto = "hola";
console.log(texto.toUpperCase());
```

## 9. Entrada de datos

- `prompt()`: permite pedir información al usuario desde el navegador.
- El valor recibido suele ser texto.

```javascript
let nombre = prompt("¿Cómo te llamas?");
console.log(`Hola ${nombre}`);
```

## 10. Operadores

### Numéricos

- `+`: suma dos valores.

```javascript
let suma = 1 + 2;
```

- `-`: resta dos valores.

```javascript
let resta = 1 - 2;
```

- `*`: multiplica dos valores.

```javascript
let multiplicacion = 1 * 2;
```

- `**`: eleva una variable a otra.

```javascript
let exponente = 1 ** 2;
```

- `/`: divide y devuelve decimales.

```javascript
let division = 1 / 2;
```

- `%`: devuelve el resto de una división.

```javascript
let modulo = 1 % 2;
```

### Comparación

- `==`: compara si dos valores son iguales.

```javascript
let a = 5;
let b = 8;
console.log(a == b);
```

- `!=`: compara si dos valores son diferentes.

```javascript
let a = 5;
let b = 8;
console.log(a != b);
```

- `>`: compara si una variable es mayor que otra.

```javascript
let a = 5;
let b = 8;
console.log(a > b);
```

- `<`: compara si una variable es menor que otra.

```javascript
let a = 5;
let b = 8;
console.log(a < b);
```

- `>=`: compara si una variable es mayor o igual que otra.

```javascript
let a = 5;
let b = 8;
console.log(a >= b);
```

- `<=`: compara si una variable es menor o igual que otra.

```javascript
let a = 5;
let b = 8;
console.log(a <= b);
```

### Lógicos

- `&&`: comprueba que dos condiciones son correctas.

```javascript
console.log(true && false);
```

- `||`: comprueba que al menos una condición es correcta.

```javascript
console.log(true || false);
```

- `!`: devuelve lo contrario de una condición.

```javascript
console.log(!true);
```

### Asignación

- `=`: asigna un valor.

```javascript
let variable = 1;
```

- `+=`: suma y asigna el resultado.

```javascript
let variable = 1;
variable += 1;
```

- `-=`: resta y asigna el resultado.

```javascript
let variable = 1;
variable -= 1;
```

- `*=`: multiplica y asigna el resultado.

```javascript
let variable = 1;
variable *= 2;
```

- `/=`: divide y asigna el resultado.

```javascript
let variable = 1;
variable /= 2;
```

- `%=`: calcula el módulo y asigna el resultado.

```javascript
let variable = 1;
variable %= 2;
```

### Identidad

- `===`: comprueba si dos valores son iguales y del mismo tipo.

```javascript
let a = [1, 2];
let b = a;
console.log(a === b);
```

- `!==`: comprueba si dos valores son diferentes o de distinto tipo.

```javascript
let a = [1, 2];
let b = [1, 2];
console.log(a !== b);
```

### Pertenencia

- `in`: comprueba si una propiedad existe en un objeto.

```javascript
let persona = { nombre: "Ana" };
console.log("nombre" in persona);
```

### BITS

- `&`: comprueba bit a bit si ambos son 1.

```javascript
let a = 3;
let b = 1;
console.log(a & b);
```

- `|`: comprueba bit a bit si al menos uno es 1.

```javascript
let a = 3;
let b = 1;
console.log(a | b);
```

- `^`: comprueba bit a bit si ambos son diferentes.

```javascript
let a = 3;
let b = 1;
console.log(a ^ b);
```

- `~`: cambia los valores bit a bit y muestra el resultado contrario.

```javascript
let a = 3;
console.log(~a);
```

- `>>`: desplaza los bits a la derecha y rellena con 0.

```javascript
let a = 3;
console.log(a >> 1);
```

- `<<`: desplaza los bits a la izquierda y rellena con 0.

```javascript
let a = 3;
console.log(a << 1);
```

## 11. Estructuras de control

### Condicionales

- `if`: ejecuta un bloque si la condición es verdadera.
- `else`: ejecuta otro bloque si la condición no se cumple.
- `else if`: añade más condiciones intermedias.

```javascript
let edad = 18;

if (edad >= 18) {
  console.log("Eres mayor de edad");
} else {
  console.log("Eres menor de edad");
}
```

```javascript
let numero = 5;

if (numero > 0) {
  console.log("Es positivo");
} else if (numero === 0) {
  console.log("Es cero");
} else {
  console.log("Es negativo");
}
```

### Bucles

- `for`: repite una acción un número fijo de veces.
- `while`: repite una acción mientras se cumpla una condición.

```javascript
for (let i = 0; i < 10; i++) {
  console.log(i);
}
```

```javascript
let contador = 0;
while (contador <= 10) {
  console.log(contador);
  contador += 1;
}
```

## 12. Manejo de excepciones

- `try`: intenta ejecutar un bloque de código.
- `catch`: ejecuta otro bloque si ocurre un error.
- `finally`: se ejecuta siempre, haya o no error.

```javascript
try {
  JSON.parse("texto no válido");
} catch (error) {
  console.log("Se ha producido un error");
} finally {
  console.log("Fin del bloque");
}
```

## 13. Clases

- `class`: permite definir un tipo con propiedades y métodos.
- Se crean objetos a partir de una clase.

```javascript
class Persona {
  constructor(nombre) {
    this.nombre = nombre;
  }
}

let persona = new Persona("Ana");
console.log(persona.nombre);
```

## 14. Módulos

- `import`: permite reutilizar código desde otros archivos.
- Se usa junto con `export` en los módulos.

```javascript
export function sumar(a, b) {
  return a + b;
}
```

## 15. Ejercicios

Para practicar lo aprendido, puedes hacer varios ejercicios y retos de programación en la siguiente página:

[Roadmap de Retos de Programación | by MoureDev](https://retosdeprogramacion.com/roadmap)
