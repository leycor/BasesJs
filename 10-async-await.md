### Async - Await


```javascript
// El async convierte la función en una promesa
const getImagen = async () => {
    const apiKey = 'C1khQe3Z7R1W2lfTO9myKeuShdqFYSGC';

    try {
        /*El await le dice a la promesa, que necesita esperar que esta termine antes de ejecutar
        la siguiente linea de codigo, una vez termine se puede pensar que el codigo es sincrono */
        const resp = await fetch(`http://api.giphy.com/v1/gifs/random?api_key=${ apiKey }`);
        const { data } = await resp.json();
        
        const { url } = data.images.original;

    } catch (error) {
        //Manejo de error
    }
}
```
