# Produccion Solar y PVGIS

Los datos de produccion solar en Suntropy se obtienen de **PVGIS** (Photovoltaic Geographical Information System), una plataforma financiada por la Comision Europea que proporciona datos de radiacion solar y produccion fotovoltaica para Europa y Africa.

## Como calcula PVGIS la produccion

PVGIS utiliza las **coordenadas geograficas** de la instalacion para calcular la produccion horaria esperada, teniendo en cuenta:

- **Radiacion solar** de la zona
- **Orientacion de los paneles (azimut)**: Sur = 0 grados, Oeste = 90 grados, Este = -90 grados, Norte = +/-180 grados
- **Inclinacion** de los paneles
- **Perdidas** del sistema

PVGIS tambien puede **optimizar la orientacion e inclinacion** optima de los paneles cuando se selecciona esta opcion en Suntropy.

## Visualizacion de datos de produccion

En el paso 5 (Resultados) se muestran los datos desglosados en **hasta 6 periodos tarifarios (P1-P6)** segun la tarifa ATR, con agregacion mensual:

### Tabla de produccion/consumo por periodos
- Produccion total por superficie y por periodo (P1-P6)
- Consumo neto por periodo
- Porcentaje de cobertura solar por periodo
- Excedentes por periodo
- Si hay baterias: energia almacenada y delta de capacidad por periodo

### Vistas disponibles
- **Produccion total agregada**: Vista mensual con grafico de barras
- **Produccion por superficie**: Contribucion individual de cada superficie
- **Vista en el Inspector**: Datos detallados para analisis en profundidad
- **Descarga en Excel**: Exportar los datos para uso externo

### Datos adicionales en Resultados
- Consumo bruto vs autoconsumo
- Excedentes
- Ahorro (gasto inicial vs gasto final)
- Porcentaje de autoconsumo anual

Los datos de produccion horaria tambien se utilizan internamente para el [[baterias-y-optimizacion|calculo de baterias]] y el balance economico.

## Seleccion de inversor

En el paso 4 tambien se selecciona el inversor. Si el plugin de **recomendacion automatica de inversor** esta activado, Suntropy sugiere el mas apropiado. Si no, se muestra la lista de inversores del [[inventario]] con un codigo de colores:
- **Verde**: Inversor optimo para la instalacion
- **Amarillo**: Inversor aceptable pero no ideal
- **Rojo**: Inversor no recomendable (aunque se puede seleccionar igualmente)

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `Autoconsumo Individual (1).pdf` - Video "Como configurar Suntropy para calcular la Produccion Solar" con demostracion del paso 4: seleccion de inversor con codigo de colores, calculo de produccion solar, adicion de baterias con criterios de optimizacion
> - `FAQ Suntropy (1).pdf` - Explicacion de PVGIS, referencias de orientacion (Sur=0, Oeste=90, Este=-90, Norte=180), y optimizacion de orientacion e inclinacion
