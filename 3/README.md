# Problemas
Los siguientes ejercicios seran calificados no solamente con el resultado, se calificara como esta desarrollado el codigo, no se acepta el uso de ciclos for ni while (2 puntos menos c/u). Se calificara que validaciones tienen para cuando se haga un caso no esperado. Es decir, si hay un metodo que suma dos enteros: `y+x` se restaran puntos si no se valida que `x` o `y` sean exclusivamente enteros.

## Ejercicio
Escriba una clase **SuperList** que contará con los siguientes criterios:
- Debe tener los siguientes Fields:
    - `Content`: El contenido de la lista.
    - `Count`: Conteo de el valor mas repetido de la lista.
    - `Type`: Tipo de lista que es, String, Int, Float, etc.    
- Tambien, debera contar con los siguientes metodos:
    - `Show()` : mostrar el contenido de la lista.
    - `Sort(order=1)`: En el caso de que sea una lista no ordenada, regresar la lista ordenada, si es una lista ordenada, imprimir que ya esta ordenada la lista. El argumento opcional `order` indicara el orden, si es 1 va en ascendente, si es 0 va en descendente.
    - `merge(list[])`: Añadir una nueva lista a la lista que tenemos, se añadiran por orden, es decir, si hay `a=[1,4,3,2]` y tengo mi objeto `SuperList.Content() > [0,1,2,3]` al hacer `merge(a)` > tendre [0,1,2,3,4], evitando valores repetidos.
    - `remove(list[])` : Removera el contenido de la lista `a` (del ejemplo anterior) a nuestra SuperList.


### Consideraciones
- **TODO** lo que involucre un ciclo, deberá de estar desarrollado con recursiones. Si se encuentran ciclos for o while se restaran puntos (2 puntos por cada ciclo)
- Se debe validar que si no se ingresan valores como se esperan, el codigo no falle, puede hacer uso de try-catch, raise Execption o LogError.