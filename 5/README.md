# Problemas
Los siguientes ejercicios seran calificados no solamente con el resultado, se calificara como esta desarrollado el codigo, no se acepta el uso de ciclos for ni while (2 puntos menos c/u). Se calificara que validaciones tienen para cuando se haga un caso no esperado. Es decir, si hay un metodo que suma dos enteros: `y+x` se restaran puntos si no se valida que `x` o `y` sean exclusivamente enteros.

## Ejercicio
Escriba una clase **GoodNumber** que contará con los siguientes criterios:
- Debe tener los siguientes Fields:
    - `Number`: El numero a revisar 
    - `Count`: Conteo de el digito mas repetido en el numero.
    - `IsGood`: Indicador de si el contenido es bueno o no.
    - `IndexValidation`: La definicion de que indices se consideran para ser validados. Puede ser pares o nones.    
- Tambien, debera contar con los siguientes metodos:
    - `new(a)` : Actualizar la lista con un nuevo numero.
    - `Show()` : mostrar el contenido de la lista.
    - `Validate()` : Revisara si el numero que se tiene es un "GoodNumber" un good number esta definido a partir del `IndexValidation` y de una validacion extra. Para el index Validation se pueden tener dos casos: 
        - Sus indices pares corresponden con un digito par. Ejemplo: 672 > el `index[0]=6` y el `index[2]=2` ambos, el 6 y 2 son pares, por lo que es correcto.
        - Sus indices pares no corresponden con un digito par. 
    - La validacion extra es que en los indices no pares(nones), deben de validar que sea un numero primo.     

### Consideraciones
- **TODO** lo que involucre un ciclo, deberá de estar desarrollado con recursiones. Si se encuentran ciclos for o while se restaran puntos (2 puntos por cada ciclo)
- Se debe validar que si no se ingresan valores como se esperan, el codigo no falle, puede hacer uso de try-catch, raise Execption o LogError.