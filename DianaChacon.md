# Information

- Nombre: **Diana Chacón Ocariz**
- Usuario Discord: **DianaChacon**
- Grupo de Lectura: **3**

# Solución

### 1. Ejercicio 1:

1) El código devuelve:

    <pre>
    console.log(numero_1); 
    -> // 2
    </pre>

    *numero_1* es una constante y su valor no cambia.

2) Como *numero_1* es una constante, si la condición del *if* fuese verdadera, *numero_1 = 3* daría error, pues una constante no puede ser modificada.


### 2. Ejercicio 2:

El código devuelve:

    console.log(numero_4); 
    -> // 7

El *numero_4* dentro del *if* es diferente al *numero_4* fuera de él. 
El primero solo tiene alcance dentro del *if*, por eso el resultado.


### 3. Ejercicio 3:

El código da error porque la variable *value* está definida dentro del *if* y
por lo tanto su alcance se limita a esta instrucción, fuera del *if*, no existe,
por lo tanto, la última instrucción falla al no conocerse *value*.

Para corregir este error, basta con declarar la variable *value* fuera del *if*:

    let value = 22;
    
    if (key == 22){
    
**Simplificaciones:**

Varias cosas se pueden simplificar en el código:

1) La constante *url_base* puede ser eliminada ya que no es utilizada.
 
2) Las instrucciones: 

        value = value + 1;
        console.log('Valor = ' + value);

        value = value - 1;
        console.log('Valor = ' + value);
        
    Son redundantes y no aportan nada, pues están seguidas.
 
 3) La condición:
    <pre>
    if (key == 22)
    </pre>
    Jamás se va a cumplir, pues *key* es una constante diferente de 22.

Propongo 2 opciones de simplificación:

1) **Solución 1:**
    <pre>
    const key = 'uahgysgkjhdsyt';
    const user_key = 'user_prueba';
    let value = 22;

    console.log('Usuario: ' + user_key + ' - Llave: ' + key);
    console.log('Valor = ' + value);
    </pre>

2) **Solución 2:**
    <pre>
    let value = 22;
    console.log('Valor = ' + value);
    </pre>
    
    Esta solución se aplicaría en el caso de que se eliminara completamente el bloque *if* que nunca se va a ejecutar dado el valor de *key*.
    
# Screenshot

#### Resultado Ejercicio 1
![Resultado Ejercicio 1](/images/Reto1-Ejercicio1.png)

#### Resultado Ejercicio 2
![Resultado Ejercicio 2](/images/Reto1-Ejercicio2.png)

#### Resultado Ejercicio 3

**Antes de corrección:**

![Resultado Ejercicio 3](/images/Reto1-Ejercicio3.png)


**Simplificación 1:**

![Simplificación 1 Ejercicio 3](/images/Reto1-Ejercicio3-corregido.png)


**Simplificación 2:**

![Simplificación 2 Ejercicio 3](/images/Reto1-Ejercicio3-corregido2.png)


# Preguntas (opcional)

**- ¿Qué aprendiste resolviendo el reto?**

Tener más clara la noción del alcance de una variable.

**- ¿Qué te gustaría reforzar?**

Por ahora creo que vamos bien :smiley:
