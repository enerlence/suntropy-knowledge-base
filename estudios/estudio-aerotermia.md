# Estudio de Aerotermia

Tipo de estudio para dimensionar y presupuestar instalaciones de aerotermia. Se accede seleccionando "Estudio Aerotermia" en el selector de tipo de estudio (arriba a la derecha del dashboard).

## Flujo del estudio (4 pasos)

### Paso 1 - Datos del cliente
- Nombre del estudio/cliente
- Provincia
- Tarifa de acceso (ej. 2.0 TD, 3.0 TD)
- Precios de energia por periodos (P1, P2, P3...)
- Datos opcionales: CUPS, DNI/CIF, direccion, email, telefono, sector
- Al completar los campos obligatorios (provincia, tarifa, precios), se habilita la flecha verde para continuar

### Paso 2 - Seleccion de aerotermia
Parametros del inmueble:
- Superficie en m2
- Tipo de vivienda (unifamiliar, etc.)
- Tipo de aislamiento
- Numero de estancias
- Numero de plantas
- Numero de residentes

Suntropy calcula una **potencia recomendada** basada en estos datos y muestra las aerotermias del [[inventario]] que esten entre el 80% y 120% de esa potencia. Se puede seleccionar cualquier otro equipo del inventario.

Se puede configurar:
- Calefaccion
- Agua caliente sanitaria (ACS)
- Enfriamiento

### Paso 3 - Calculo de ahorros
- Seleccionar el sistema de calefaccion actual del cliente (gasoleo, gas natural, propano, electrico, etc.)
- Introducir el gasto anual en calefaccion del cliente
- Suntropy calcula el **ahorro anual por sustitucion de combustible**

**Calculo del consumo de aerotermia:**
Se basa en un patron de uso: horas/dia por mes x potencia x rendimiento = consumo en kWh

Se puede:
- Modificar los inputs (horas de uso) por mes
- Usar perfiles predeterminados (uso moderado, alto, etc.)
- Crear perfiles personalizados por mes y estacion

La curva de consumo horaria resultante se usa para calcular el ahorro comparando con el combustible actual.

### Paso 4 - Balance economico
- Precio de la instalacion (puede venir predefinido del kit/pack de aerotermia cargado en inventario)
- Descuentos
- Subvenciones
- Condiciones de financiacion
- Se pueden asociar [[editor-de-plantillas|plantillas de presupuesto]] con configuracion condicional basada en parametros de aerotermia (ej. metros cuadrados)

## Integracion con autoconsumo

La curva de consumo de aerotermia generada en el paso 3 se puede importar dentro de un estudio de [[autoconsumo-individual]] para calcular el ahorro combinado de autoconsumo fotovoltaico + aerotermia. Esto se hace a traves del plugin de complementos de consumo.

## Kits de aerotermia

A diferencia de los kits solares (paneles + inversor), los kits de aerotermia asocian la aerotermia con conceptos adicionales cargados como [[equipos-personalizados]], creando un pack completo.

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `Aerotermia (2).pdf` - Transcripcion del Crash Course de aerotermia con videos paso a paso:
>   - "Datos del Cliente en un Estudio de Aerotermia" - Video detallado del paso 1
>   - "Selecciona la Aerotermia en el Estudio" - Video del paso 2 con explicacion de calculo de potencia recomendada, tipos de aislamiento, seleccion de calefaccion/ACS/enfriamiento, y kits de aerotermia
>   - "Calcula los Ahorros en el Estudio de Aerotermia" - Video del paso 3 con explicacion detallada del patron de uso, perfiles predeterminados y calculo del ahorro por sustitucion de combustible
>   - "Genera el Balance Economico de la instalacion de Aerotermia" - Video del paso 4 con detalle de financiacion y plantillas condicionales
