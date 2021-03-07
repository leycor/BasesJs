### Promesas

Una promesa representa un valor que puede estar disponible: ahora, en un futuro o nunca.


```javascript

const promesa = new Promise( (resolve, reject)=>{

    //Función que recibe un callBack y permite ejecutar una tarea en cierto tiempo 
    setTimeout( ()=>{
        resolve();
    }, 2000 )
});

promesa.then( ()=>{
    console.log('Then de la promesa')
})
```

> Cómo se puede observar una promesa es una función de flecha que recibe dos parametros `resolve` se ejecutará en caso de que la promesa pase de manera correcta, mientras qué `reject` se ejecutará en caso de que falle