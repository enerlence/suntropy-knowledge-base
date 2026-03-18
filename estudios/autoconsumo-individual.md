# Autoconsumo Individual

Estudio fotovoltaico para un unico punto de suministro. Es el tipo de estudio principal y mas utilizado en Suntropy.

## Flujo del estudio (6 pasos)

### Paso 1 - Datos del cliente
- Nombre del estudio/cliente
- Provincia (determina radiacion solar via PVGIS)
- Tarifa de acceso a la red (ATR): 2.0 TD, 3.0 TD, 6.X TD, etc.
- Precios de energia por periodos (P1, P2, P3...)
- Precios de potencia contratada
- Datos opcionales: CUPS, DNI/CIF, direccion, email, telefono, sector
- Se pueden introducir [[precios-alternativos]] si se quiere proponer un cambio de tarifa

### Paso 2 - Consumo
Introduccion de la [[curvas-de-consumo|curva de consumo]] del cliente. Metodos disponibles:
- **Patrones de consumo** (~90% de usuarios): Integrado con REE, genera curva horaria segun zona y tarifa ATR
- **Facturas**: Introduccion manual por periodos
- **Importar curva CSV/Excel**: Para datos SIPS o curva horaria real. Necesario para tarifas 6.X TD
- **Datadis**: Importacion directa si esta [[integraciones|integrado]]

Plugins adicionales en este paso:
- **Complementos de consumo**: Anadir consumo de aire acondicionado, coche electrico, aerotermia
- **Trasladar consumo**: Desplazar un porcentaje del consumo a horas determinadas (util para estudios comerciales)

### Paso 3 - Seleccion de superficie
- Dibujar la superficie de paneles sobre el mapa (Google Maps/satelite)
- Definir orientacion (azimut) e inclinacion de los paneles
- Seleccionar el [[kits-coplanares|kit solar]] (coplanar o no coplanar segun inclinacion)
- Anadir [[sombras-y-obstaculos|obstaculos y analisis de sombras]]
- [[optimizacion-potencia|Optimizacion de potencia]] disponible con 5 criterios

### Paso 4 - Produccion
- Datos obtenidos de [[produccion-solar-pvgis|PVGIS]]
- Visualizacion por periodos tarifarios (P1-P6)
- Produccion total, por superficie, y en Inspector
- Descarga en Excel disponible

### Paso 5 - Resultados
- Tabla de produccion/consumo por periodos
- Porcentaje de cobertura solar por periodo
- Excedentes por periodo
- Si hay baterias: energia almacenada y delta de capacidad
- Consumo bruto vs autoconsumo
- Ahorro (gasto inicial vs gasto final)
- Porcentaje de autoconsumo anual

### Paso 6 - Balance economico
- Precio de la instalacion
- Seleccion de [[excedentes-y-retribucion|modalidad de excedentes]]: vertido a red, PPA, inyeccion 0, bateria virtual
- Descuentos y subvenciones
- Condiciones de financiacion (integracion con [[integraciones|Pontio]] disponible)
- [[equipos-personalizados]] como partidas adicionales
- [[intervalos-potencia|Plantillas de intervalo de potencia]] para calculo automatico del precio
- Calculo del ROI (ver [[roi-retorno-inversion]])
- [[baterias-y-optimizacion|Optimizacion de baterias]]

## Guardar y compartir
- Se puede [[guardar-estudio-incompleto|guardar en cualquier momento]] sin completar todos los pasos
- El estudio se puede compartir con el cliente mediante enlace unico
- Se puede rastrear visualizaciones del presupuesto compartido (cuantas veces se ha visto, por cuanto tiempo, cuantas veces se ha compartido)
- Los [[estados-estudios|estados]] permiten clasificar el ciclo de vida del estudio
- Se puede ver toda la cronologia del estudio: cuando fue creado, compartido, enviado, etc.
- Se puede aprobar a companeros del equipo para que vean el estudio

## Formas de calcular el precio

En el paso 6, el precio de la instalacion se puede calcular de tres formas:
1. **Precio llave en mano**: Se introduce directamente el precio total
2. **Presupuesto avanzado**: Suma automatica de precios del inventario (paneles + inversores + baterias + equipos personalizados). Requiere tener el plugin activado
3. **Ratio euro/vatio pico**: Se introduce el ratio y se calcula automaticamente segun la potencia del estudio

Tambien se puede anadir un **margen comercial** (porcentaje sobre el coste) para empresas que cargan precios de coste en el inventario.

## Tipo de instalacion

Es importante seleccionar si la instalacion es **monofasica** o **trifasica**, ya que afecta a la seleccion de inversores.

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `Autoconsumo Individual (1).pdf` - Transcripcion del Crash Course de autoconsumo individual con videos paso a paso:
>   - "Rellena los Datos de la Seccion Cliente" - Video del paso 1, incluye detalle de tipo de instalacion monofasica/trifasica
>   - "Genera la Curva de Consumo Horaria de tus Clientes" - Video del paso 2 con demostracion practica de patrones de consumo REE, complementos y trasladar consumo
>   - "Selecciona la Superficie de la Instalacion Fotovoltaica" - Video del paso 3 con detalle de integracion catastral, zoom ampliado, Ctrl+C/V de paneles, distancia filas/columnas, analisis de sombras con escala de colores, multiples superficies
>   - "Como configurar Suntropy para calcular la Produccion Solar" - Video del paso 4 con seleccion automatica de inversor (plugin), colores verde/amarillo/rojo, calculo de baterias
>   - "Evalua los Resultados de Produccion de la Instalacion Fotovoltaica" - Video del paso 5 con graficos y datos de ahorro
>   - "Calcula el Balance Economico" - Video del paso 6 con las 3 formas de calcular precio, margen comercial, retribucion de excedentes, financiacion con Pontio, compartir estudio y rastreo de visualizaciones
> - `FAQ Suntropy (1).pdf` - Preguntas frecuentes con detalles adicionales sobre curvas REE, PVGIS, optimizacion, sombras, excedentes y estados
