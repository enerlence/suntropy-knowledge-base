# Editor de Plantillas de Presupuesto

El editor de plantillas permite crear y personalizar los presupuestos que se generan para los clientes. Se accede desde **Herramientas > Plantillas**.

## Funcionalidades del editor

### Tema
Desde el icono del pincel se puede modificar:
- Colores del presupuesto
- Logotipo de la empresa

### Componentes disponibles
- **Graficas**: Graficos de produccion, consumo, ahorro, etc.
- **KPIs**: Indicadores clave del estudio
- **Superficie de paneles**: Visualizacion de la disposicion de paneles
- **Textos editables**: Texto libre personalizable
- **Textos parametricos**: Textos con formulas dinamicas que se rellenan automaticamente con datos del estudio (nombre del cliente, potencia, ahorro, etc.)
- **Imagenes**: Imagenes estaticas o del estudio
- **Videos**: Embeber videos (ej. explicativos)
- **Imagen de [[equipos-personalizados|equipo personalizado]]**: Mostrar imagenes de equipos adicionales

### Fondos de pagina
Se pueden subir disenos como fondo para cada pagina del presupuesto.

### Configuracion condicional
Se puede hacer que componentes, paginas completas o incluso plantillas enteras aparezcan o no segun condiciones del estudio:
- Si hay financiacion
- Si hay bateria
- Segun la tarifa del cliente
- Segun otros parametros del estudio

### Operaciones con componentes
- **Duplicar** componentes desde el engranaje de cada uno
- **Eliminar** componentes
- **Ajustar margenes y esquinas** para posicionar y dar forma

## Editor vs Visor

**Importante**: El editor de plantillas (donde se crea la plantilla base) es diferente del visor de plantillas (donde se hacen ajustes puntuales para un estudio especifico sin modificar la plantilla base).

## Recomendaciones

- **Guardar frecuentemente** los cambios mientras se edita
- Usar configuracion condicional para tener una sola plantilla que se adapte a diferentes tipos de estudios

## Tipos de plantilla

Al crear una nueva plantilla se puede elegir:
- **Vertical**: Formato clasico de documento
- **Horizontal**: Formato apaisado
- **Landing page**: Formato interactivo con botones (mas moderno y web)

## Texto parametrico con calculo

El componente de texto parametrico permite no solo mostrar datos del estudio, sino tambien hacer **calculos sobre formulas**. Se pueden ejecutar sumas, restas, multiplicaciones y divisiones sobre cualquier parametro (ej. aplicar un descuento al importe PVP, calcular un porcentaje de devolucion, etc.).

Las formulas se dividen en:
- **Parametros del estudio** (datos introducidos por el usuario): nombre del cliente, tarifa, precio, ubicacion, direccion, etc.
- **Parametros calculados** (datos generados por Suntropy): ahorro mensual, ahorro total, coste de la instalacion, ROI, etc.

## Presupuesto manual

Ademas del componente automatico de presupuesto, se puede crear un presupuesto completamente manual usando:
- **Formas** (rectangulos) como cabeceros y separadores
- **Textos editables** con titulos de columnas (Descripcion, Unidades, Precio)
- **Textos parametricos** con formulas de paneles, inversores, numeros de unidades, garantias, etc.
- Esto permite total libertad de formato y diseno

## Margenes y esquinas redondeadas

Los margenes permiten deslizar componentes con precision mas alla de la rejilla base. Los radios de esquinas permiten redondear los bordes de componentes para un aspecto mas moderno.

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `Plantillas (1).pdf` - Transcripcion completa del Crash Course del editor de plantillas con 9 videos:
>   - "La importancia de una propuesta personalizada" - Introduccion al valor comercial de personalizar plantillas
>   - "Edita el tema y anade fondos al Editor de plantillas" - Como modificar colores principales/secundarios y logotipo, usar codigos de color de la marca, y como los colores se aplican automaticamente a graficas y textos
>   - "Anade componentes dentro de la plantilla" - Tipos de componentes (basicos, cliente, consumo, graficas, KPIs, superficie), previsualizacion, personalizacion de titulos, leyendas, colores, modo compacto en superficie, ocultar/mostrar elementos
>   - "Conoce todas las opciones del Componente de texto" - Editor de texto tipo Word (negrita, tipografia, tamano, colores primario/secundario), formulas dinamicas (parametros del estudio vs parametros calculados), margenes y radios de esquinas
>   - "Componente de texto Parametrico" - Calculadora de formulas: sumas, restas, multiplicaciones, divisiones sobre parametros del estudio (ejemplo: descuento sobre importe PVP), previsualizacion en tiempo real, numero de decimales
>   - "Crea una Configuracion Condicional en componentes, paginas y plantillas" - 3 niveles de condiciones: por componente (ej. pago contado vs financiacion), por pagina (ej. mostrar solo si hay bateria), por plantilla (ej. aplicar segun tarifa ATR o financiacion). Incluye ejemplos practicos
>   - "Disena una partida de materiales de forma manual" - Como crear un presupuesto personalizado con formas, textos editables y formulas (panel, inversor, estructura, precios, garantias)
>   - "Anade los Equipos Personalizados a la plantilla" - Como usar texto parametrico con formulas de equipos personalizados e imagen de equipo personalizado. Importante: activar la opcion para que aparezcan
>   - "Diferencia entre el Editor y Visor de plantillas" - Editor (crear plantilla base desde Herramientas>Plantillas) vs Visor (ajustes puntuales desde un estudio, sin modificar la base). Importante: guardar como "editado" antes de generar/compartir
