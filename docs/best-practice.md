# Best Practice

[Clean Code](https://github.com/jhonPariona/clean-code/blob/master/README.md#clean-code)

## Editor

**usar 4 espacios de identación**

**Límite de 79 caracteres en cada línea**

## Modularizar

- Reutilizar parte de códigos, eneralizar y consolidad código repetido en funciones y bucles.
- Usar el min número de entities(clases, modulos, funciones)

## Variables

**usar `_` para separar identificadores de variables**

```python
declaration_var = "asignation var"
```

**escribir nombres significativos(meaningful)** y descriptivos pero solo con información relevante

## Booleans vars

**Usar prefijos** `is_` o `has_`

## Listas

**Agregar el tipo de variable que es siempre en cuando exista otra variable similar**

```python
age_list = []

for age in age_list:
  print(age)
```

**Evitar(avoid) abreviaturas** a exepción de contadores en for o abreviaturas generales que entiendan los que leen el codigo

## Funciones

- Deben de realizar una única función
- podemos usar parámetros generales ejem. `arr` para arrays
- Tratar de usar menos de 3 parámetros


## 📖 Documentación

Texto adicional o info ilustrada incrustada en el código

- Útil para el esclarecimiento de partes complejas del código.

### Tipos

**In-line** Deben usarse para código que sea complicado de explicar mediante el código mismo. ejemplo: El por qué un método se implementó de una manera específica.

```python
# comment in-line
```

**[Docstrings](https://www.python.org/dev/peps/pep-0257/)** Se realiza a nivel de una función, es considerado una buena práctica. Si la función es simple basta con indicar únicamente una descripción y omitir los Args y Returns.

```python
def population_density(population, land_area):
    """Calculate the population density of an area.

    Args:
    population: int. The population of the area
    land_area: int or float. This function is unit-agnostic, if you pass in values in terms of square km or square miles the function will return a density in those units.

    Returns:
    population_density: population/land_area. The population density of a 
    particular area.
    """
    return population / land_area
```

**Project DOcumentation** Por que y como su código es relevante para otro y si es que podrian ser potenciales usuarios o contribuidores. Se usa el README para esto.

EL README debe contener:

- Explicar que el lo que hace
- Lista de dependencias
- Instrucciones detalladas sobre como usarlo

## Pruebas

### Pruebas Unitarias

Se realizan a una unidad de código(funciones)

⚙️ **Tools**

- **[pytest](https://docs.pytest.org/en/latest/getting-started.html)**
  - Los archivos deben nombrarse `tes_<nameTest>.py`
  - Las funciones de los test tambien deben de empezar con `tes_`
  - [configuracion](https://docs.pytest.org/en/latest/customize.html)
  
### TDD(Test-driven-development)

Escribir los test antes de escribir código.

- Los tests deben representar todos los posibles escenarios que se nos ocurran

### Logging

Registrar mensajes descriptivos de los eventos que ocurrieron en nuestra aplicación

- Ser claros
- Ser concisos
- Usar de manera adecuada las mayúsculas
- Proveer únicamente información útil donde, cuando, cómo, ...
- Elegir de manera adecuada el nivel para el log
  - Debug: todo lo que sucede en la aplicación
  - Error: Registra los errores que se producen
  - Info: específico del sistema del usuario
  
### Code Reviews

Ayuda a mejorar el código para su puesta en producción, se realiza por otro desarrollador.

- Revizar si se están cumpliendo las buenas prácticas
- Realizar comentarios de sugerencias y no mandatos.
- Evitar usar en los comentarios "yo" o "tu" en vez de eso usar nosotros
- proporcionar código de ejemplo en los comentarios
- Usar un linter y una guia de estilo establecido por e grupo
  - pylint
