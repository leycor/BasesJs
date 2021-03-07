### Fetch Api

La API Fetch proporciona una interfaz para recuperar recursos, la forma de obtener estos es mediante la siguiente sintaxis:

```javascript

// Api Key privada
const apiKey = 'C1khQe3Z7R1W2lfTO9myKeuShdqFYSGC';

// Esta constante al tener fetch retorna un Response lo cual significa que es una promesa
const peticion = fetch(`http://api.giphy.com/v1/gifs/random?api_key=${ apiKey }`);

peticion
    .then( resp => resp.json() )
    .then( ({ data }) => {
        const { url } = data.images.original;
    })
    .catch( console.warn );
```