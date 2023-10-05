<!-- No borrar o modificar -->
[Inicio](./index.md)

## Actividad 3 

**Listas**
### Crea una lista que contenga los números del 1 al 10.
### Imprime la lista en el orden en que fue creada.
### Ordena la lista en orden ascendente.
### Ordena la lista en orden descendente.
### Encuentra el número más pequeño en la lista.
### Encuentra el número más grande en la lista.
### Cuenta el número de veces que aparece el número 5 en la lista.
### Elimina el número 5 de la lista.
### Agrega el número 11 a la lista.
### Imprime la lista nuevamente.

```

lista = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
print(lista)
lista.sort()
print(lista)
lista.reverse()
print(lista)
numeroMenor = min(lista)
print(numeroMenor)
numeroMayor = max(lista)
print(numeroMayor)
numeroVeces = lista.count(5)
print(numeroVeces)
lista.remove(5)
lista.append(11)
print(lista)```

```
**Tuplas**
### Crea una tupla que contenga las palabras "Hola", "mundo" y "Python".
### Imprime la tupla en el orden en que fue creada.
### Ordena la tupla en orden alfabético.
### Encuentra la primera palabra en la tupla.
### Encuentra la última palabra en la tupla.
### Cuenta el número de palabras en la tupla.
### Elimina la palabra "mundo" de la tupla.
### Agrega la palabra "Hola" a la tupla.
### Imprime la tupla nuevamente.

```
tupla = ("Hola", "mundo", "Python")
print(tupla)
#no es posible ordenar en nombre alfabetico
print(tupla)
print(tupla[0])
print(tupla[-1])
numeroVecest = len(tupla)
print(numeroVecest)
# no es posible eliminar
# no es posible agregar
print(tupla)

```

**Conjuntos**
### Crea un conjunto que contenga los números del 1 al 10.
### Imprime el conjunto.
### Agrega el número 11 al conjunto.
### Elimina el número 5 del conjunto.
### Cuenta el número de elementos en el conjunto.
### Comprueba si el número 5 está en el conjunto.
### Comprueba si el número 11 está en el conjunto.
### Crea un conjunto que contenga las palabras "Hola", "mundo" y "Python".
### Imprime el conjunto.
### Comprueba si la palabra "Hola" está en el conjunto.
### Comprueba si la palabra "mundo" está en el conjunto.

```
conjunto = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}
print(conjunto)
conjunto.add(11)
print(conjunto)
conjunto.remove(5)
print(conjunto)
largo = len(conjunto)
print(largo)
print(5 in conjunto)
print(11 in conjunto)
conjuntoPal = {"hola", "mundo", "python"}
print(conjuntoPal)
print("hola" in conjuntoPal)
print("mundo" in conjuntoPal)

```
**Diccionarios**
### Crea un diccionario que asigne los nombres de los días de la semana a sus números correspondientes.
### Imprime el diccionario.
### Obtén el número del día de la semana "Lunes".
### Obtén el día de la semana del número 2.
### Elimina el día de la semana "Lunes" del diccionario.
### Imprime el diccionario nuevamente.

```
semana = {"domingo":1, "lunes":2, "martes":3, "miercoles":4, "jueves":5, "viernes":6, "sabado":7}
print(semana)


lunes = semana.get("lunes")
print(lunes)

for llave, valor in semana.items():
    if (valor == 2):
        print(llave)

semana.pop("lunes")
print(semana)

```