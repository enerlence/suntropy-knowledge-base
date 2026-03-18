# Optimizacion de Potencia

La optimizacion de potencia en Suntropy permite encontrar automaticamente la configuracion optima de paneles para una superficie segun un criterio seleccionado.

## Como funciona

1. Se determina el **kit de mayor potencia** (o numero maximo de paneles) que cabe fisicamente en la superficie definida
2. Desde ese maximo, el sistema **itera hacia abajo**, reduciendo paneles y comprobando en cada paso si se cumple el criterio de optimizacion
3. Se detiene cuando encuentra la configuracion que cumple el criterio

## Criterios de optimizacion (5 modos)

| Criterio | Descripcion | Valor de entrada |
|----------|-------------|------------------|
| **Numero maximo de meses con excedentes** | Limita cuantos meses al ano la produccion mensual puede superar al consumo mensual | Numero de meses (ej. 3) |
| **Porcentaje maximo de excedentes** | Comprueba que no se generan mas excedentes que el porcentaje indicado respecto a la produccion total. Permite ajustes mas granulares | Porcentaje (ej. 15%) |
| **Porcentaje de ahorro energetico** | Determina la potencia pico para alcanzar un porcentaje objetivo de ahorro en energia (kWh ahorrados respecto al consumo total) | Porcentaje (ej. 50%) |
| **Porcentaje de ahorro economico** | Determina la potencia pico para alcanzar un porcentaje objetivo de ahorro economico (euros ahorrados respecto a la factura actual) | Porcentaje (ej. 40%) |
| **Porcentaje de consumo total** | Determina la potencia pico para que la produccion cubra un porcentaje del consumo total. Puede superar el 100% (sobreproduccion) | Porcentaje (ej. 80%) |

## Opciones adicionales del modo "Ahorro economico"

Cuando se selecciona el criterio de ahorro economico, se pueden activar tres opciones que afinan el calculo:

- **Considerar retribucion de excedentes**: Incluye la compensacion por excedentes vertidos a red en el calculo del ahorro economico
- **Usar precios alternativos**: Utiliza los [[precios-alternativos]] (si se han introducido) en lugar de los precios actuales del cliente
- **Considerar termino de potencia**: Incluye los costes del termino de potencia contratada en el calculo del ahorro economico

## Recomendacion

- Para una optimizacion basica y rapida: usar los modos de excedentes (porcentaje o meses)
- Para optimizacion mas completa con impacto economico real: usar el modo de ahorro economico con sus opciones adicionales
- Para afinar mas: el modo de porcentaje maximo de excedentes permite variaciones mas pequenas que el de meses

## Limites de superficies

No existe limite de superficies en un estudio, pero al aumentar mucho el numero de superficies, el proceso de optimizacion se ralentizara.

## Parametros predeterminados

Los parametros de optimizacion de potencia pico se pueden predeterminar en **Configuracion > Estudios de autoconsumo** para que se apliquen por defecto a todos los estudios nuevos.

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `FAQ Suntropy (1).pdf` - Explicacion detallada de como funciona la optimizacion (iteracion desde maximo hacia abajo), diferencia entre modos de meses vs porcentaje de excedentes, y recomendacion de cual es mas preciso
> - `Configuracion (2).pdf` - Video "Conoce todas las configuraciones de tu perfil de usuario" donde se explican los parametros predeterminados de optimizacion en Configuracion > Estudios de autoconsumo
