A Ema le gusta vivir viajando, se la pasa yendo de ciudad en ciudad. 

En la parte de "Biblioteca" se definen tres ciudades. En este modelo, los objetos que representan ciudades saben responder a cuatro cosas  

- `haySol()`: devuelve un booleano.
- `cantidadMuseos()`: devuelve un número.
- `costoTransporte()`: devuelve un número.
- `costoHotel()`: devuelve un número.

Se nos pide que programemos el objeto que representa a Ema, que debe entender estos mensajes: 

- `gastosDiarios()`: devuelve un número que es la estimación de cuánto gasta Ema por día. Esto es la suma del costo de hotel y el costo de transporte de la ciudad donde esté, más 500 pesos para otros gastos.
- `estaComoda()`: devuelve un booleano que indica si Ema está cómoda. Para que esto pase, la ciudad donde está debe cumplir dos condiciones: tiene que haber sol, y tiene que tener más de 5 museos.
- `mudarse(ciudad)`: mediante este método se informa que Ema se muda a la ciudad indicada en el argumento. El efecto de este mensaje es realizar una acción, no devuelve ningún valor.

P.ej. la siguiente secuencia debe funcionar como se indica

```wollok
>>> ema.mudarse(encarnacion)
>>> ema.gastosDiarios()
3550
>>> ema.estaComoda()
false
>>> ema.mudarse(salvadorDeBahia)
>>> ema.gastosDiarios()
3200
>>> ema.estaComoda()
true
```

En esta secuencia, la primera vez que se le pregunta a Ema si está cómoda, responde que no porque la ciudad donde está, Encarnación, no cumple la condición de los museos.  
La segunda vez responde que sí, porque Salvador de Bahía cumple las dos condiciones que pide Ema.

