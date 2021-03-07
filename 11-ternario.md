### Condicional ternario

Se trata de otra forma de crear condicionales de una manera mas simplificada

```javascript

const activo = true;

// Condicional de dos respuesta
const mensaje = ( activo ) ? 'Activo' : 'Inactivo';

// Condicional de una respuesta
const mensaje = activo && 'Activo';
```
> `?` Es lo que retornará si la respuesta es `true`
> `:` Es lo que retornará si la respuesta es `false`
> `&` Solo retornará un elemento si la respuesta es true o false, dependiendo la condicion que se le coloque



console.log(mensaje);