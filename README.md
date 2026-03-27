## Estado del Workflow ✅

![CI](https://github.com/MatiasMoragaAS/Taller-4-Matias-Moraga/actions/workflows/workflow.yml/badge.svg)

# Correcciones en functions.py
como realiza la correcion antes de subirlo no aparece. lo agrego por escrito

en functions.py
# add(a, b)

se elimino str quedando 
```
def add(a, b):
    return (a + b)
``` 
# divide(a, b)
se elimino el + 1 y los parentesis
```
def divide(a, b):
    return a / b
```
# def get_element(list_, index):
  se elimino el + 1
```
def get_element(list_, index):
    return list_[index]
```
# convert_to_integer(value)
se agrego int 
```
def convert_to_integer(value):
    return int(float(value))
```
# en workflow
borre la especificacion que el workflow corra solo en la rama main 

```
on:
  push:
  pull_request:
```

agrege la instalacion de pytest 
```
 - name: Install dependencies
      run: pip install pytest
```
y cambio de version actuales de las actions

de  actions/checkout@v2 -> actions/checkout@v4
y actions/setup-python@v2 -> actions/setup-python@v5










