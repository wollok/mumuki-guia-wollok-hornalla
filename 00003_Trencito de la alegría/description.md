Ahora nos piden hacer un modelo del trencito de la alegría, que entienda estos mensajes:

- `vaCargado()`: verdadero si lleva más de 40 pasajeros, falso en caso contrario.
- `vaTranca()`: verdadero si lleva menos de 10 pasajeros, falso en caso contrario.
- `subir(cant)`: aumenta la cantidad de pasajeros en lo que indica `cant`, un número.
- `bajar(cant)`: disminuye la cantidad de pasajeros en lo que indica `cant`, un número.
- `vaciar()`: deja al trencito sin pasajeros.

Lo que sigue es un ejemplo del comportamiento que se espera.

```wollok
>>> trencito.vaciar()       // no tiene ningún pasajero
>>> trencito.vaCargado()    
false
>>> trencito.vaTranca()
true
>>> trencito.subir(25)      // ahora tiene 25 pasajeros
>>> trencito.vaCargado()    
false
>>> trencito.vaTranca()
false
>>> trencito.subir(20)      // ahora tiene 45 pasajeros
>>> trencito.vaCargado()    
true
>>> trencito.vaTranca()     // falso
false
>>> trencito.bajar(38)      // ahora tiene 7 pasajeros
>>> trencito.vaCargado()
false
>>> trencito.vaTranca()     
true
```

Otra vez, es importante descubrir cuántos atributos se necesitan, y de qué característica.
