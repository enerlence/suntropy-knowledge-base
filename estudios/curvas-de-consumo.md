# Curvas de Consumo

Las curvas de consumo (o curvas de carga) son la representacion horaria del consumo electrico del cliente a lo largo de un ano. Se introducen en el **paso 2** del estudio de autoconsumo.

## Metodos de introduccion

### 1. Patrones de consumo (la mas usada, ~90% de usuarios)
- Seleccionar "Patrones de consumo" > "Domestico" o "Comercial"
- Suntropy esta integrado con los perfilados de **Red Electrica Espanola (REE)**
- REE genera una curva horaria estadisticamente representativa segun la zona geografica y la tarifa ATR del cliente
- Seleccionar el ultimo ano completo e introducir el consumo mensual o anual
- **Limitacion**: REE **no genera perfilados para tarifas 6.X TD**. Para estas tarifas es necesario usar una curva real

### 2. Facturas
- Introduccion manual de consumos por periodos de facturacion
- Se pueden agregar uno o todos los meses

### 3. Importar curva de consumo (CSV/Excel)
- Descargar la plantilla compatible desde Suntropy
- Rellenar con datos horarios de consumo
- Establecer fecha de inicio y fecha de fin del periodo de datos
- Cargar el archivo completado
- Util cuando se tiene acceso a datos SIPS o a la curva horaria real del punto de suministro
- **Necesario para tarifas 6.X TD**

### 4. Datadis
- Requiere estar dado de alta en Datadis y tener la [[integraciones|integracion configurada]]
- Importa la curva de consumo directamente desde la base de datos de distribuidoras

## Plugins que modifican la curva

### Complementos de consumo
Permite anadir consumo adicional a la curva:
- Aire acondicionado
- Coche electrico
- Aerotermia

### Trasladar consumo
Desplaza un porcentaje del consumo a unas horas determinadas. Util para estudios comerciales donde se quiere simular un cambio en el patron de consumo.

## Por que se usan los perfiles de REE

Los perfilados de REE se emplean porque no es comun disponer de una curva de carga horaria real. Con los perfilados, se distribuye el consumo total (mensual o anual) en las horas en las que se produce de forma estadisticamente representativa para esa zona y tarifa. Esto genera una curva horaria casi exacta para la mayoria de tarifas.

## Visualizacion de la curva

Una vez generada la curva, se puede visualizar:
- En formato de **barras mensuales** (enero, julio, agosto y diciembre suelen tener mayor consumo)
- Los **patrones de consumo horarios** (distribucion a lo largo del dia)

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `Autoconsumo Individual (1).pdf` - Video "Genera la Curva de Consumo Horaria de tus Clientes" con demostracion practica de como seleccionar patrones domesticos/comerciales, introducir consumo mensual o anual, visualizar la curva en barras, activar complementos de consumo y trasladar consumo
> - `FAQ Suntropy (1).pdf` - Explicacion de por que se usan perfilados de REE y la limitacion con tarifas 6.X TD
