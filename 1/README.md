# Problemas
Los siguientes ejercicios seran calificados no solamente con el resultado, se calificara como esta desarrollado el codigo, no se acepta el uso de ciclos for ni while (2 puntos menos c/u). Se calificara que validaciones tienen para cuando se haga un caso no esperado. Es decir, si hay un metodo que suma dos enteros: `y+x` se restaran puntos si no se valida que `x` o `y` sean exclusivamente enteros.

## Ejercicio
Escriba una clase **Palindrome** que contará con los siguientes criterios:
- Debe tener los siguientes Fields:
    - Size: Tamaño del palindromo.
    - Count: Conteo de la letra que mas se repite y su valor.
    - Palindrome: donde se almacena el palindromo.
    - Value: donde se contiene el valor si no es palindromo.
- Tambien, debera contar con los siguientes metodos:
    - Show() : mostrar el palindromo o el contenido.
    - isPalindrome(): Revisar si es un palindromo.
    - new(value) : cambiar el palindromo actual con un nuevo valor.
    - remove(index=0) : eliminar un elemento en un indice definido, este metodo debera de mantener la estructura de un palindromo. Es decir "anitalavalatina" > remove(2) = "antalavalatna".
    - add(index=0) : agregar un nuevo elemento en un indice definido. Tambien debe mantener la estructura de un palindromo.
    - multiply(n) : Se repetira el palindromo n veces, actualizando sus fields, size, count, palindrome, value.


### Consideraciones
- Un palindromo es una palabra que se puede escribir igual en ambas direcciones: 
    - anitalavalatina
    - oxxo
    - lol
- **TODO** lo que involucre un ciclo, deberá de estar desarrollado con recursiones. Si se encuentran ciclos for o while se restaran puntos (2 puntos por cada ciclo)
- Para los metodos remove y add, puede no escribirse un valor de indice, es decir, estar vacio, el valor por defecto debe ser 0.
- Si se hace uso del metodo `new(value)` y el valor de **value** no es un palindromo, se debe agregar en el field **value** pero, si es un palindromo, se guardara en **Palindrome** 