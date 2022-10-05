# Problemas
Los siguientes ejercicios seran calificados no solamente con el resultado, se calificara como esta desarrollado el codigo, no se acepta el uso de ciclos for ni while (2 puntos menos c/u). Se calificara que validaciones tienen para cuando se haga un caso no esperado. Es decir, si hay un metodo que suma dos enteros: `y+x` se restaran puntos si no se valida que `x` o `y` sean exclusivamente enteros.

## Ejercicio
Escriba una clase **Brackets** que contará con los siguientes criterios:
- Debe tener los siguientes Fields:
    - `brackets`: El string completo.
    - `Count`: Conteo de la cantidad de brackets completos que tiene.
    - `Type`: Conteo de los tipos de brackets que tiene, el maximo es 3:`(,[,{`.
    - `Values`: string donde se contiene el valor si no es bracket.
- Tambien, debera contar con los siguientes metodos:
    - `Show()` : mostrar el contenido de brackets.
    - `isComplete()`: Revisar si lo contenido en brackets tiene brackets completos.
    - `indexes()`: Mostrar los indices en donde se muestran los brackets, es decir, si tengo la siguiente expresion:
    `[hola(dios{soy yo(de nuevo)})]` se debe regresar: (0:29,5:28,16:27,17:26)
    - `remove(index=0)`: Removera el contenido y los brackets, tomando el ejemplo anterior, `remove(index=17)` > `[hola(dios{soy yo})]`


### Consideraciones
- Un bracket completo es aquel que tiene un inicio y un cierre, es decir: `[({()})]` ese tiene 4 brackets completos, sin embargo `[({(})]` este solamente tiene 3 completos
- **TODO** lo que involucre un ciclo, deberá de estar desarrollado con recursiones. Si se encuentran ciclos for o while se restaran puntos (2 puntos por cada ciclo)
- Se debe validar que si no se ingresan valores como se esperan, el codigo no falle, puede hacer uso de try-catch, raise Execption o LogError.