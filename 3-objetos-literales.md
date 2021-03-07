### Objetos Literales

Dado un objeto podemos crear una copia del mismo usando la siguiente sintaxis
```javascript

const persona = {
    nombre: 'Tony',
    apellido: 'Stark',
    edad: 45,
    direccion: {
        ciudad: 'New York',
        zip: 55321321,
        lat: 14.3232,
        lng: 34.9233321
    }
};

// Copia de objeto persona
const persona2 = { ...persona };
 ```



