<!-- No borrar o modificar -->
[Inicio](./index.md)

## Actividad 3 

**Listas** 

1. Crea una lista que contenga los números del 1 al 10.
2. Imprime la lista en el orden en que fue creada.
3. Ordena la lista en orden ascendente.
4. Ordena la lista en orden descendente.
5. Encuentra el número más pequeño en la lista.
6. Encuentra el número más grande en la lista.
7. Cuenta el número de veces que aparece el número 5 en la lista.
8. Elimina el número 5 de la lista.
9. Agrega el número 11 a la lista.
10. Imprime la lista nuevamente.

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
1. Crea una tupla que contenga las palabras "Hola", "mundo" y "Python".
2. Imprime la tupla en el orden en que fue creada.
3. Ordena la tupla en orden alfabético.
4. Encuentra la primera palabra en la tupla.
5. Encuentra la última palabra en la tupla.
6. Cuenta el número de palabras en la tupla.
7. Elimina la palabra "mundo" de la tupla.
8. Agrega la palabra "Hola" a la tupla.
9. Imprime la tupla nuevamente.

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
1. Crea un conjunto que contenga los números del 1 al 10.
2. Imprime el conjunto.
3. Agrega el número 11 al conjunto.
4. Elimina el número 5 del conjunto.
5. Cuenta el número de elementos en el conjunto.
6. Comprueba si el número 5 está en el conjunto.
7. Comprueba si el número 11 está en el conjunto.
8. Crea un conjunto que contenga las palabras "Hola", "mundo" y "Python".
9. Imprime el conjunto.
10. Comprueba si la palabra "Hola" está en el conjunto.
11. Comprueba si la palabra "mundo" está en el conjunto.

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
1. Crea un diccionario que asigne los nombres de los días de la semana a sus números correspondientes.
2. Imprime el diccionario.
3. Obtén el número del día de la semana "Lunes".
4. Obtén el día de la semana del número 2.
5. Elimina el día de la semana "Lunes" del diccionario.
6. Imprime el diccionario nuevamente.

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