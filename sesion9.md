<!-- No borrar o modificar -->
[Inicio](./index.md)

## Sesión 9 
```
import pandas as pd
import streamlit as st
import matplotlib.pyplot as plt 
data = pd.read_csv('ventas_vehiculos .csv')

st.dataframe(data)
```
# Eliminar valores faltantes
```
data = data.dropna()
```
# valores atípicos 
```
data = data[(data['Precio'] > 1000) & (data['Precio'] < 100000)]
data = data[~((data["Kilometraje"] > 100.000) & (data["Estado"] == "Nuevo"))]
data = data[data["Año"]>2000]
```

# Eliminar datos duplicados
```
data = data.drop_duplicates()
```

# Convertir el formato 
```
data['Año'] = data['Año'].astype(int)
```
```
st.title("Histograma de Precios")
plt.hist(data['Precio'], bins=20)
st.pyplot()
```

### Documentacion


**Valores Atípicos:**

1.Se identificaron valores de precio que estaban fuera del rango típico para vehículos, se aplica un filtro para mantener solo las filas donde el precio estaba entre 1000 y 100,000.

2.Se eliminan registros donde el "Kilometraje" es mayor a 100,000 y el "Estado" es "Nuevo", ya que los vehículos nuevos generalmente no tendrían un kilometraje tan alto. 

3.Se están eliminando los vehículos cuyo año de fabricación sea anterior a 2000, ya que son muy pocos a comparacion de los despues del 2000


**Formato Incorrecto en el Año:**
 Se convirtió la columna 'Año' al formato entero utilizando astype(int).