# Baterias y Optimizacion

El calculo de baterias en Suntropy se realiza a partir de las curvas horarias de produccion y consumo, comparando hora a hora la energia generada con la demandada.

## Parametros del calculo

- **Capacidad inicial (%)**: Estado de carga inicial de la bateria al comenzar el analisis
- **Capacidad minima (%)**: Limite inferior de descarga (protege la vida util de la bateria)
- **Capacidad maxima (%)**: Limite superior de carga (evita sobrecargas)

## Criterios de optimizacion

### 1. Excedentes totales (%)
Porcentaje de la energia excedente que puede ser almacenado en la bateria. Un valor alto indica uso eficiente de los excedentes y buen dimensionamiento.

### 2. Porcentaje de autoconsumo (%)
Mide la independencia energetica: que parte de la energia consumida proviene de la instalacion (produccion solar + bateria). Mayor porcentaje = menor dependencia de la red.

### 3. Dias de autonomia
Dias que el sistema podria funcionar solo con la bateria, sin produccion solar. Especialmente relevante para instalaciones aisladas o para resiliencia energetica ante fallos de red.

## Proceso de optimizacion

1. El sistema evalua las diferentes baterias del [[inventario]]
2. Simula el balance energetico con cada una (teniendo en cuenta capacidad, profundidad de descarga, eficiencia, etc.)
3. Filtra las que cumplen los criterios minimos establecidos por el usuario
4. Si ninguna bateria del inventario cumple los criterios, el sistema lo informa

## Anadir baterias al inventario

Las baterias se cargan en **Herramientas > [[inventario]] > Baterias** con los siguientes datos:
- Capacidad (kWh)
- Profundidad de descarga (%)
- Eficiencia (%)
- Fabricante y modelo
- Precio

## Detalle del balance horario

Para cada hora se comparan produccion y consumo:

- **Produccion < Consumo**: La energia generada cubre parte de la demanda. La diferencia se intenta cubrir con la bateria. Si la bateria no tiene suficiente carga, se recurre a la red.
- **Produccion > Consumo**: La demanda se satisface completamente. El excedente carga la bateria. Si la bateria esta llena, la energia sobrante se vierte a la red.

## Visualizacion

Al calcular baterias en el paso 4, se muestra:
- Excedentes almacenados
- Energia almacenada total
- Grafico de excedentes vs almacenamiento mensual

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `Calculo de baterias.pdf` - Documento tecnico con explicacion detallada del algoritmo de calculo horario de baterias: escenarios produccion<consumo y produccion>consumo, parametros de capacidad inicial/minima/maxima, proceso de optimizacion con inventario, y descripcion completa de los 3 criterios (excedentes totales, porcentaje de autoconsumo, dias de autonomia)
> - `Autoconsumo Individual (1).pdf` - Video "Como configurar Suntropy para calcular la Produccion Solar" con demostracion de como anadir baterias en el paso 4, seleccionar packs y ver resultados graficos
