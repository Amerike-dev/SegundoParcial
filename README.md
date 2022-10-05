# Instrucciones
1. Lea **TODAS EL CONTENIDO** de este README.
2. Abra la carpeta con el numero asignado en la clase para resolver el parcial.
3. Lea el archivo README.md contenido en la carpeta.
4. Realize un script que vaya asignado a un empty gameobject.
5. Realize el push a este repositorio en la rama master.

## Consideraciones
Realizar el push unicamente en la carpeta asignada.

## Criterios de calificacion:
Hasta el momento hemos programado de forma informal. Se ha realizado codigo dejando la mayoria de las veces variables publicas y no se ha hecho uso de los campos (fields) y propiedades (properties).

- Un **argumento opcional** es un parametro que puede o no estar al llamar una funcion, este se escribe `method(name:value)` y en donde se define el metodo/funcion, debe estar declarado el valor for defecto
```
public void method(string name="")
{
    ...
}
```
Ese metodo esta esperando un string para usarlo como variable local `name`, sin embargo, si no le mandan nada entonces inicializara un valor vacio. Esto aplica en cualquier argumento.  

- Un **Field** es un elemento de la clase que guarda valores propios de la clase en si. Este elemento es una caracteristica propia de la clase, se conocen como "Properties" pero se deben llamar **Fields**.  Se suelen escribir **_field** y son privados.

- Una **Property** te deja acceder a los fields, y suelen tener una validacion. Sirven de capa para que no se pueda modificar codigo directamente. Se suelen escribir publicos y con su **get** y **set** correspondiente.

Codigo de ejemplo
```
public class MyClass
{
    private string _myField;

    public string MyProperty
    {
        get
        {
            return _myField;
        }
        set
        {
            _myField = value;
        }
    }
}
```
Pareceria que no tienen mucho proposito, pero se usan las **properties** para validar los tipos de dato o asignar valores a varios **fields**

```
public class MyClass
{
    private int _myField1;
    private int _myField2;
    private int _myField3;

    public Vector2 MyProperty1
    {
        get { return new Vector2(_myField1, _myField2); }
        set
        {
            _myField1 = value.x;
            _myField2 = value.y;
        }
    }

    public int MyProperty2
        get { return _myField3;}
        set
        {
            if(value > 0)
            {
                myField3 = value;
            }
            else
            {
                LogError("Values for _myField3 must be possitive");
            }
        }
}
```
El codigo que realizaran para el examen debe de utilizar **Fields** y **Properties** si no lo tiene, entonces se tendran puntos menos.
