### Arreglos en JS

Un arreglo es una lista de elementos y la forma de declararlo en JS es la siguiente:

```javascript
const arreglo = [1,2,3,4];

// Para agregar un nuevo elemento en un arreglo utilizaremos el operador spread el cual crea una copia del arreglo anterior y agrega al final el elemento que coloques.
const arreglo2 = [ ...arreglo, 5 ];

```

### Metodo `.map()`

Este método nos permite iterar todos los elementos de un arreglo, retornando un nuevo arreglo,
dada una determinada función o callback a ejecutar en cada elemento que lo compone.

```javascript

const myArray = [10, 20, 30];
const newArray = myArray.map(number => number + 1);
newArray;
// Prints [11, 21, 31]
```

> Como podemos ver, estamos diciendo que por cada elemento en myArray, debemos ejecutar la siguiente función number => number + 1.(En este caso utilizamos un arrow function).


forEach()
/* Este método, similar al map(), ejecutará el callback indicado por cada elemento del arreglo.
La mayor diferencia entre ambos, es que este método no retorna un nuevo arreglo y solo se limitará a recorrerlo. */
const myArray = [10, 20, 30];
const myArray.forEach(number => calculateSomething(number);

reduce()
/* Este método nos permite, dada una función, “reducirlo” o “transformar” los elementos de un arreglo en un nuevo y único valor. */
var myArray = [10, 20, 30];
var total = myArray.reduce((accumulator, number) => {
 return accumulator + number;
});
total;
// Prints 60

/* Como podemos ver, nuestra función se ejecutará por cada elemento del arreglo, esperando dos parametros,
un acumulador y el elemento actual, el acumulador se encargara (como indica su nombre) de acumular el resultado final
luego de cada operación. Si no se provee un valor inicial al acumulador,
su valor inicial será el valor del primer elemento del arreglo. */

find()
// Este método nos retornara el primer elemento que encuentre cumpliendo los requerimientos que proponga nuestro callback.
const myArray = [{number: 10}, {number: 20}, {number: 30}, {number: 40}];
const singleValue = myArray.find(el => el.number === 30);
singleValue
// Prints {number: 30}

/* Como podemos ver, nuestro callback se ejecutará con cada elemento del arreglo, recibiendo 
el elemento actual y luego retornando true o false dada una condición que nosotros determinemos, 
si es true, dará por terminada la iteración y nos retornará ese valor que cumple la condición. Si es false, 
continuará con el siguiente elemento. */

filter()
/* Método con funcionamiento similar al de find(), retornara un nuevo arreglo con todos los elementos
que encuentre cumpliendo los requerimientos que proponga nuestro callback. */
const myArray = [10, 20, 30, 40];
const filteredValues = myArray.filter(number => number > 20);
filteredValues
// Prints [30, 40]