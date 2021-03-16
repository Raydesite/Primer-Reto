# Information

- **Nombre: Daniel Jaramillo G**
- **Usuario Discord: JaraDaniel#6764**
- **Grupo de Lectura: Lectura 3**

# Solución

#### Ejercicio 1: Solución
El valor que tendrá `numero_1` al final del script es de 2.
La razón es que es una constante. Además, en el caso hipotético en el que `número_1` fuese inicializado con el valor de 6 
y el programa entrara al if statement, el programa arrojaría un error porque estamos intentando reasignar un valor a una constante
y que además su tipo de dato es primitivo (en este caso `Number`).


#### Ejercicio 2: Solución
El valor que tendrá `numero_4` al final del script es de 7.
En primer lugar, el valor de `numero_1` no es 6 y en el caso hipotético que así fuera, 
la variable declarada como `numero_4` sería valida únicamente dentro del statement if,
es decir dentro de su scope, luego de esto ya no existiría.

#### Ejercicio 3: Solución

```
const url_base = 'https://api.prueba.com';
const key = 'uahgysgkjhdsyt';
const user_key = 'user_prueba';
let value = 22;

if (value === 22){
	console.log('Usuario: ' + user_key + ' - Llave: ' + key);
	console.log('Valor = ' + value);

	value++;
	console.log('Valor = ' + value);

  value--;
	console.log('Valor = ' + value);

}

console.log('Valor = ' + value);

```

# Screenshot

Agrega un screenshot de tu resultado o resultados (si son varios ejercicios agrega un título a cada screenshot).

# Preguntas (opcional)

- ¿Qué aprendiste resolviendo el reto?
  Practiqué todo lo referente al scope.

- ¿Qué te gustaría reforzar?
Me gustaría reforzar la cohersión de tipos
