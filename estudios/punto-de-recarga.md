# Punto de Recarga para Vehiculo Electrico

Suntropy permite incluir puntos de recarga para vehiculos electricos de tres formas distintas.

## Opcion 1 - Estudio independiente (3 pasos)

1. Seleccionar **"Punto de recarga"** en el selector de tipo de estudio (arriba a la derecha)
2. **Paso 1**: Introducir datos del cliente (nombre, provincia, tarifa de acceso)
3. **Paso 2**: Seleccionar el cargador individual o kit de punto de recarga del [[inventario]]
4. **Paso 3**: Configurar el presupuesto con [[equipos-personalizados]], descuentos, subvenciones y condiciones de financiacion

## Opcion 2 - Complemento de consumo en estudio de autoconsumo

Usar el plugin **"Complementos de consumo"** (activar en Configuracion > [[plugins]]):
- En el paso 2 del estudio de [[autoconsumo-individual]], seleccionar "Coche electrico" como complemento
- Se anade el consumo mensual del cargador a la curva de consumo del estudio
- Permite dimensionar la instalacion solar teniendo en cuenta el consumo del vehiculo electrico

## Opcion 3 - Equipo personalizado en balance economico

Anadir el cargador como [[equipos-personalizados|equipo personalizado]] en el paso 6 (Balance Economico) del estudio de autoconsumo, sumandolo al presupuesto final sin afectar al calculo energetico.

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `Punto de Recarg vehiculo electrico (1).pdf` - Transcripcion del Crash Course de punto de recarga con videos:
>   - "Anadir un Punto de Recarga para V.E." - Video introductorio con las 3 formas de incluir punto de recarga
>   - "Crea un presupuesto de Punto de Carga para V.E." - Video paso a paso del estudio independiente: seleccion de cargador del inventario, kits de punto de recarga, plantillas de presupuesto automaticas, equipos personalizados, descuentos (ej. descuento navideño con opcion anual), subvenciones, condiciones de financiacion (ejemplo BBVA 7% 120 cuotas), generacion de PDF y compartir enlace
