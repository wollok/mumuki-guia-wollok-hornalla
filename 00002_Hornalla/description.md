Lo que se pide en este ejercicio parece fácil: modelar una hornalla de gas. 

La temperatura de la hornalla es: 180 grados si está prendida, 20 grados si está apagada.

El consumo de gas es: 4 dm3 si está prendida, 0 dm3 si está apagada.

La definición del objeto `hornalla` debe incluir estos cuatro métodos:

- `temperatura()`: devuelve un número de acuerdo a lo explicado arriba.
- `consumo()`: devuelve un número de acuerdo a lo explicado arriba.
- `prender()`: no devuelve ningún valor, realiza una acción.
- `apagar()`: no devuelve ningún valor, realiza una acción.

El objeto debe funcionar como se indica abajo:

```wollok
>>> hornalla.prender()
>>> hornalla.temperatura()   
180
>>> hornalla.consumo()
4
>>> hornalla.apagar()
>>> hornalla.temperatura()   
20
>>> hornalla.consumo()
0
```

Para que el modelo de hornalla funcione correctamente, hay que incluir variables. ¿Cuántas? Alcanza con una. Si te sale con dos variables está OK, pero mejor si usás una sola.

