# Plantillas de Intervalo de Potencia

El plugin de Plantillas de Intervalo de Potencia permite a las empresas que calculan el precio final de su instalacion a traves de un **ratio euro/vatio pico (euros/Wp)** crear rangos de precios escalonados.

## Como configurar

1. Activar el plugin en **Configuracion > [[plugins|Plugins]]**
2. Crear plantillas de intervalos definiendo rangos de potencia y su ratio asociado

### Ejemplo de rangos

| Rango de potencia | Ratio |
|-------------------|-------|
| De 0 a 5 kWp | 1.50 euros/Wp |
| De 5 a 10 kWp | 1.30 euros/Wp |
| De 10 a 15 kWp | 1.10 euros/Wp |
| De 15 a 20 kWp | 0.90 euros/Wp |

## Uso en estudios

En el paso 6 (Balance Economico) del [[autoconsumo-individual|estudio de autoconsumo]], se activa un boton que aplica automaticamente el ratio de la plantilla de potencia configurada segun la potencia pico del estudio.

Esto automatiza el calculo del precio sin tener que escribirlo manualmente cada vez.

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `Configuracion (2).pdf` - Video "Domina todos los Plugins de Suntropy" con demostracion de como crear y editar plantillas de intervalo de potencia con rangos personalizados y como se aplica el boton en el balance economico
