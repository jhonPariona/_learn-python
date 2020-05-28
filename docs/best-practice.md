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

