# Problemas
Los siguientes ejercicios seran calificados no solamente con el resultado, se calificara como esta desarrollado el codigo, no se acepta el uso de ciclos for ni while (2 puntos menos c/u). Se calificara que validaciones tienen para cuando se haga un caso no esperado. Es decir, si hay un metodo que suma dos enteros: `y+x` se restaran puntos si no se valida que `x` o `y` sean exclusivamente enteros.

## Ejercicio
Escriba una clase **Elimination** que contará con los siguientes criterios:
- Debe tener los siguientes Fields:
    - `Content`: El contenido de la lista.
    - `Count`: Conteo de el valor mas repetido de la lista.
    - `Order`: El orden en que realizará la eliminacion, ascendente o descendente.
    - `Size` : El tamaño de la lista.
    - `Interval`: El intervalo en el que hara las eliminaciones.
- Tambien, debera contar con los siguientes metodos:\
    - `new(a)` : Actualizar la lista con una nueva `a[]`.
    - `Show()` : mostrar el contenido de la lista.
    - `Eliminate()`: El proceso de eliminar, usando order e interval, se hara la eliminacion de los elementos que tenga la lista.     
    Ejemplo:
    `[1, 43, 3, 0, 2, 10, 34]` con `order=ascendente` e `interval=2`
    resultado = `[1, 43, 0, 2, 34]` eliminamos cada 2 elementos. empezando de izquierda a derecha
    - `add(index=0)`: Añadir una nuevo elemento a la lista que tenemos, si hay un indice definido añadirlo en donde marca, sino, por default es 0.
    - `remove(index=0)` : Removera el elemento contenido de la lista, con el mismo criterio que add().


### Consideraciones
- **TODO** lo que involucre un ciclo, deberá de estar desarrollado con recursiones. Si se encuentran ciclos for o while se restaran puntos (2 puntos por cada ciclo)
- Se debe validar que si no se ingresan valores como se esperan, el codigo no falle, puede hacer uso de try-catch, raise Execption o LogError.