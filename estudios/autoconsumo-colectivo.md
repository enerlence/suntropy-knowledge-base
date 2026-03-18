# Autoconsumo Colectivo

Estudio para dimensionar instalaciones fotovoltaicas compartidas entre multiples consumidores (comunidades de vecinos, edificios con locales comerciales, etc.).

## Flujo del estudio

### 1. Introducir consumidores
- Anadir cada participante con sus datos: nombre, direccion, DNI/CIF, email
- Agrupar consumidores en **perfiles** (ej. "Residentes", "Locales comerciales")
- Cada perfil tiene: tarifa, perfil de consumo y consumo medio definidos

### 2. Curva de consumo agregada
- Suntropy genera las curvas de consumo individuales automaticamente
- Se genera la curva total agregada de todos los participantes

### 3. Seleccion de superficie
- Dibujar la superficie de la instalacion sobre el mapa
- Se puede ver la distancia desde cada consumidor a la superficie
- Radio maximo: **2 km** para autoconsumo colectivo (requisito regulatorio)

### 4. Produccion y coeficientes de reparto
Se calcula la produccion solar y se selecciona la estrategia de reparto:

| Estrategia | Descripcion |
|------------|-------------|
| **Equitativo** | Todos reciben la misma proporcion (1/N) |
| **Proporcional al consumo** | Mayor participacion a quien mas consume en cada hora. Maximiza el ahorro global |
| **Personalizado** | Se define manualmente el coeficiente por perfil |
| **Optimizacion de ahorro** | Busca la combinacion optima de coeficientes dinamicos (en desarrollo) |

### 5. Balance economico
- Resultados agregados por perfil
- Resultados individuales por consumidor
- Inversion proporcional segun coeficiente de reparto

### 6. Compartir resultados
- Se genera un **enlace unico** para todos los participantes
- Cada participante accede a sus resultados individuales identificandose con su DNI/CIF, CUPS o email
- Se puede rastrear quien ha visualizado el presupuesto y durante cuanto tiempo
- Se puede enviar el enlace por correo a todos los participantes desde la propia plataforma
- Funciona en dispositivos moviles

## Introduccion de consumidores

Formas de introducir consumidores:
- **Manual**: Uno a uno, introduciendo datos y asignando a un perfil
- **Duplicar**: Se puede duplicar un consumidor ya creado para agilizar (util cuando varios tienen datos similares)
- **Proximo**: Importacion masiva desde Excel o ZIP de facturas PDF (en desarrollo)

Cada consumidor puede tener precios de energia individualizados aunque pertenezca a un perfil comun.

La relacion perfil-consumidor puede ser 1:N (un perfil para varios consumidores con consumo medio comun) o 1:1 (perfil especifico con datos individuales, incluso curva horaria propia).

## Resultados detallados

Los resultados se muestran a dos niveles:
- **Agregado por perfil**: Coeficiente total medio, produccion equivalente, excedentes y ahorro del grupo
- **Individual por consumidor**: Datos especificos de produccion, excedentes y ahorro. Si los consumidores tienen precios de energia diferentes, sus ahorros seran diferentes aunque tengan el mismo coeficiente

Se puede visualizar:
- Media horaria de coeficientes de reparto dinamicos por mes
- Balance economico a 25 anos por participante (potencia pico equivalente, inversion equivalente, ahorros con compensacion simplificada)

## Balance economico

El coste de la instalacion se puede calcular igual que en [[autoconsumo-individual]], incluyendo:
- Ratio euro/vatio pico
- [[equipos-personalizados]] y [[editor-de-plantillas|plantillas de presupuesto]]
- La inversion se reparte proporcionalmente segun coeficiente de reparto de cada participante

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `Autoconsumo Colectivo (3).pdf` - Transcripcion del Crash Course de autoconsumo colectivo con videos paso a paso:
>   - "Introduce los Perfiles de cada Cliente en un Estudio de A.Colectivo" - Video detallado de como crear consumidores, perfiles, asignar tarifas y consumos. Incluye ejemplo con 6 residentes + 2 locales comerciales
>   - "Calcula el consumo horario de los consumidores" - Video del paso 2 con curvas medias horarias por perfil y descarga en Excel
>   - "Diseno de superficies para A.Colectivo" - Video con detalle de distancias a consumidores, radio de actuacion de 2km y multiples superficies
>   - "Elige el tipo de retribucion para cada perfil en el Estudio de A.Colectivo" - Video con explicacion detallada de las 3 estrategias de coeficientes de reparto, clasificacion (optimo/justo/sencillo/personalizado) y visualizacion de coeficientes dinamicos por hora
>   - "Genera el Balance Anual y economico de la instalacion de A.Colectivo" - Video con balance por perfil y por consumidor individual a 25 anos
>   - "Comparte los resultados personalizados con cada usuario de la Comunidad de Vecinos" - Video con enlace unico, acceso por DNI/CIF, rastreo de visualizaciones por participante
