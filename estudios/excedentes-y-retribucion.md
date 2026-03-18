# Excedentes y Modalidades de Retribucion

Los excedentes son la energia producida por la instalacion solar que no se consume directamente y se vierte a la red electrica. La modalidad de retribucion se selecciona en el **paso 6 (Balance Economico)** y afecta directamente al calculo del ROI y al ahorro total proyectado.

## Modalidades disponibles

| Modalidad | Descripcion |
|-----------|-------------|
| **Vertido a red** | Los excedentes se venden a la red al precio fijado en el balance economico (en euros/MWh). Se tiene en cuenta esta retribucion en el calculo de ahorro |
| **PPA (Power Purchase Agreement)** | Se descuenta del precio de la instalacion el precio de los excedentes generados durante el periodo de vida util de la instalacion |
| **Inyeccion 0** | No se tienen en cuenta los excedentes en el calculo economico. La instalacion se dimensiona para minimizar los vertidos a red |
| **Bateria virtual** | Los excedentes se acumulan en un "monedero virtual" que se puede usar para compensar consumo futuro de la red |

## Notas importantes

- La unidad del precio de excedentes es **euros/MWh** (no euros/kWh)
- La modalidad de inyeccion 0 puede alargar el [[roi-retorno-inversion|retorno de inversion]] ya que el ahorro se basa solo en el autoconsumo directo
- La eleccion de modalidad impacta significativamente en la viabilidad economica del proyecto
- En autoconsumo colectivo, se puede seleccionar **compensacion simplificada** como modalidad

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `FAQ Suntropy (1).pdf` - Explicacion de las diferencias entre modalidades de retribucion (vertido a red, PPA, inyeccion 0)
> - `Autoconsumo Individual (1).pdf` - Video "Calcula el Balance Economico" donde se muestra como seleccionar la modalidad y configurar el precio de excedentes en euros/MWh
