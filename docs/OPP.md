# OPP

## Class

Plantilla que contiene los atributos y métodos delos obetos.

[Sintaxis clases y objetos](https://youtu.be/Y8ZVw1LHI8E)

### Self

Es un dicionario que contiene las propiedades y valores de las propiedades de una clase, se pasa como primer argumento. Self es una convencion de nombre pero se pude asar otro nombre tambien pero eso confundiría a otros programadores.

## Objects

Instance of class (instancia de una clase)

Los objetos s definen por:

**Attributes Atributos** Son characteristics(característica), property(propiedad), description(descripción), feaure(caracteistica), tarit(rasgo) que son ***nouns(SUSTANTUIVOS)***

**Methods Métodos** Son actions(acciones) que son ***verbs(VERBOS)***

[Class objects and attributes](https://youtu.be/yvVMJt09HuA)


### Diferencia Method and function

**Method** inside of a class(Dentro de una clase)

**Function** outside of a class(Fuera de una clase)


```python
class Shirt:

    def __init__(self, shirt_color, shirt_size, shirt_style, shirt_price):
        self.color = shirt_color
        self.size = shirt_size
        self.style = shirt_style
        self.price = shirt_price
    
    def change_price(self, new_price):
    
        self.price = new_price
        
    def discount(self, discount):

        return self.price * (1 - discount)
```
