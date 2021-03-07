### Desestructuración de `arrays`

Los arrays tambien los podemos desestructurar, pero cómo sus elementos no tienen una llave para poder identificarlos la manera
de acceder a esto es por medio de sus posiciones, Ej:

```javascript

const personajes = ['Goku','Vegeta','Trunks'];

/* Nuestro arrays es el siguiente
0 - Gokú
1 - Vegeta
2 -Trunks
 */

const [ , , p3 ] = personajes;
console.log( p3 );
// Print: Trunks
```
> En esta desestructuración, asignamos el nombre **p3** al elemento en la posición **numero 2**

### Ejemplo numero 2

```javascript

// Función que retorna una lista con dos elementos
const retornaArreglo = () =>{
    return ['ABC', 123];

// Desestructuramos la función para tener esos elementos separados por variables
const [ letras, numeros ] = retornaArreglo(); 
}
```