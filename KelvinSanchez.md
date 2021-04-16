# Information

- Nombre: Kelvin Sánchez
- Usuario Discord: kelvinsanchez15#6349

# Solución

1. Ejercicio 1: Solución

```js
const numero_1 = 2;

if (numero_1 == 8) {
  let numero_4 = 5;
  numero_1 = 3;
}

let numero_4 = 7;

console.log(numero_1);
```

Se imprime `2` en la consola porque la variable `numero_1` es declarada como una constante en el ámbito global y en dicho ámbito se invoca el método `console.log` con `numero_1` como parámetro.

2. Ejercicio 2: Solución

```js
const numero_1 = 2;

if (numero_1 == 6) {
  let numero_4 = 5;
  numero_1 = 3;
}

let numero_4 = 7;

console.log(numero_4);
```

Se imprime `7` en la consola ya que la variable `numero_4` fue declarada en el mismo ámbito en el que se invoca el método `console.log`. La sentencia `if` no tiene ningún efecto en el resultado
porque la condición no se cumple y en el caso de que se cumpliese la variable `numero_4` declarada dentro de ella estaría en el ambito local de la sentencia. 

3. Ejercicio 3: Solución

```js
const url_base = "https://api.prueba.com";
const key = "uahgysgkjhdsyt";
const user_key = "user_prueba";

if (key == 22) {
  let value = 22;
  console.log("Usuario: " + user_key + "- Llave: " + key);
  console.log("Valor = " + value);

  value = value + 1;
  console.log("Valor = " + value);

  value = value - 1;
  console.log("Valor = " + value);
}

console.log("Valor = " + value);
```

El código no funciona porque la variable `value` no está definida en el ámbito en cual es llamada. Esto se soluciona bien sea declarando la variable `value` fuera de la sentencia `if`
o moviendo el método `console.log` dentro.

Si queremos que se ejecute el código dentro de la condición tenemos que modificar la misma para que devuelva `true` al evaluarse.

Por último, podemos refactorizar el código usando template literals y operadores de asignación:

```js
const url_base = "https://api.prueba.com";
const key = "uahgysgkjhdsyt";
const user_key = "user_prueba";
let value = 22;

if (key == "uahgysgkjhdsyt") {
  console.log(`Usuario: ${user_key} - Llave: ${key}`);
  console.log(`Valor = ${value}`);
  console.log(`Valor = ${(value += 1)}`);
  console.log(`Valor = ${(value -= 1)}`);
}

console.log("Valor = " + value);
```

# Screenshot
1. Ejercicio 1

![reto1](https://user-images.githubusercontent.com/4708484/110868832-ae437700-829f-11eb-9fdb-4ab615721b68.png)

2. Ejercicio 2

![reto2](https://user-images.githubusercontent.com/4708484/110869433-d7183c00-82a0-11eb-8d59-8b76bc4c9c75.png)

3. Ejercicio 3

- Si no se cumple la condición:

![reto-3-1](https://user-images.githubusercontent.com/4708484/110869912-cae0ae80-82a1-11eb-91a7-9d1aa98b3c6d.png)


- Si se cumple la condición:

![reto3-2](https://user-images.githubusercontent.com/4708484/110869698-586fce80-82a1-11eb-8180-be7e57187f5c.png)
