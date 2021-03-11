# Information

- Nombre: Elmer Sorto
- Usuario Discord: Elmer#9446

## Solución

1. El resultado es 2
   En el primer ejercicio obtenemos 2 porque no le hacemos ningun cambio ya que la condición devuelve falso y no es evaluada. Aunque si la condición fuera evaluada, daría un error debido a que no se puede reasignnar una constante.

2. El resultado es 7
   En el ejercicio 2 la respuesta es 7 ya que tampoco se evalua la condición. Si pudiese evaluarse, dadría error ya que se intenta asignar valor a una variable que fue declarada constante. 
   Luego, suponiendo que todo eso esté bien, el resultado seguiría siendo 7 ya que no estamos haciendo un console.log dentro de la condición, y la variable dentro de la condición tiene un scope local.
3. No funciona porque la variable **value** no ha sido definida en el scope global, solo en el local de la condición la cual solo puede usarse en ese scope.
La solución que se me ocurre, sería definir la variable fuera de la condición.

## Screenshot

Ejercicio 1

![Ejercicio 1](https://i2.paste.pics/9681f0699620c02398db775784c63a55.png)

Ejercicio 2

![Ejercicio 2](https://i2.paste.pics/d455d4e59a084104266ba60ed58f09da.png)

Ejercicio 3: si la condicion evaluara

![Ejercicio 3: si la condicion evaluara](https://i2.paste.pics/235bf76f0924eb057f81fd40d37bc9fa.png)

Ejercicio 3: cuando no evalúa la condición

![Ejercicio 3: cuando no evalúa la condición](https://i2.paste.pics/2777f5de80aa87aa357f73d80e577672.png)

## Preguntas (opcional)

Aprendí sobre el alcance de las variables, pero me gustaría aprender un poco mas sobre ello y sobre todo sobre algo llamado **hoisting**, palabra que encontré mientras averiguaba sobre el scope.

## Código simplificado

Solo se me ocurrió hacerle estos pequeños cambios, no estoy seguro qué más podríamos simplificar.

```javascript
const url_base = 'https://api.prueba.com';
const key = 'uahgysgkjhdsyt';
const user_key = 'user_prueba';
let value = 22;

if (key == 22) {
  console.log(`Usuario:  ${user_key} - Llave:  ${key}`);

  console.log(`Valor = ${value}`);

  value +=  1;
  console.log(`Valor = ${value}`);

  value -= 1;
  console.log(`Valor = ${value}`);
}

console.log('Valor = ' + value);
```
