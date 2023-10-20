<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 10 
```
    import streamlit as st
    import pandas as pd

    data = pd.read_csv('natalidad.csv',delimiter = ";")
```

### filtro de los nacidos en el año 2021
```
    data = data[data["ANO"] == 2021]
```

### filtro de nacidos con peso igual o superior a 3500 y talla igual a 50
```
    data = data[(data['PESO_NAC'] >= 3500) & (data['TALLA_NAC'] == 50)]
```

### filtrar nombre de la clinica que contenga la palabra "PRADO"
```
    data = data[data['NOM_INST'].str.contains("PRADO", case=False)]
```

### filtro de madres menores de 18
```
    def mama_menor_de_18(EDAD_MADRE):
     return EDAD_MADRE < 18

    data = data[mama_menor_de_18(data["EDAD_MADRE"])]

```
### filtrar a edad del padre de forma descendente
```

    data2 = data.sort_values(by= "EDAD_PADRE", ascending= False)

```
### mostrar las tres primeras filas
```
    data3 = data.head(3)
```

### filtrar la segunda fila y mostrarla como tabla
```
    data4 = data.loc[2]
```

### filtrar la serie con los mayores datos
```
    data5 = data.max(numeric_only=1)
```

### filtar la serie con los datos menores
```
    data6 = data.min(numeric_only=1)
```

### Devuelve un diccionsrio con cuyas calves son
### tuplas que ressultan de todas las combinaciones de los valores de
### las columnas con nombres en la lista columnas
```
    data7 = data.groupby("BARRIO_RES").groups
```

[Registro de los nacimientos de personas residentes en el municipio de Medellín, sexo, peso,talla,tipo de parto, información de la madre](http://medata.gov.co/dataset/nacimientos)





