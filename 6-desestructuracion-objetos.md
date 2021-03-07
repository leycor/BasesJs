### Desestructuración de Objetos

La desestructuración de objeto nos ayuda a tener acceso a cada uno de los valores de este de manera directa,
de tal manera no tendremos que estar colocando de forma repetitiva el nombre del objeto mas su clave para acceder a su valor.

```javascript


const persona = {
    nombre: 'Tony',
    edad: 45,
    clave: 'Ironman'
};

// Desestructurando el objeto persona
const { edad, clave, nombre, } = persona;

console.log( edad )
// Print: 45
```
> De esta forma nos evitamos utilizar `persona.edad` para acceder a su valor.