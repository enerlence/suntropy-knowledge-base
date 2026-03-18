# Sombras y Obstaculos

Suntropy tiene en cuenta las sombras en las superficies de paneles de dos formas.

## Sombras entre filas de paneles

Se calculan automaticamente:
- Las sombras que se producen al colocar filas sucesivas de paneles
- Las sombras que los paneles generan entre si
- Se usan las dimensiones reales de los paneles para determinar cuantos caben en una superficie

## Sombras de obstaculos

En el paso 3 (Seleccion de superficie) se pueden anadir obstaculos:

1. **Dibujar obstaculos** sobre el mapa: arboles, chimeneas, edificios colindantes, muros, antenas, etc.
2. Asignar una **altura** al obstaculo
3. Ejecutar un **analisis de sombras** que simula el movimiento de la sombra a lo largo del dia y del ano
4. Visualizar mediante una **escala de colores** el porcentaje de sombra que afecta a cada panel

## Acciones tras el analisis

En base a los resultados del analisis de sombras, se puede:
- **Reubicar paneles**: Mover los paneles afectados a zonas con menos sombra
- **Colocar optimizadores**: Instalar optimizadores en los paneles parcialmente sombreados para maximizar su rendimiento
- **Eliminar paneles**: Quitar los paneles que esten demasiado sombreados y no sean rentables (con la tecla Suprimir del teclado)

## Tipos de obstaculos

Ejemplos de obstaculos que se pueden dibujar: arboles, chimeneas, edificios colindantes, muros, antenas, casetas de ascensor, etc. Se les asigna una altura y el sistema simula como se mueve la sombra.

## Simulacion anual

Al pulsar el analisis anual, la escala de colores muestra el porcentaje acumulado de sombra a lo largo de todo el ano para cada panel, permitiendo tomar decisiones informadas.

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `Autoconsumo Individual (1).pdf` - Video "Selecciona la Superficie de la Instalacion Fotovoltaica" con demostracion practica: dibujar obstaculos sobre el mapa, asignar altura (ejemplo: arbol de 8m), ejecutar simulacion hora a hora y anual, visualizar escala de colores con porcentaje de sombra por panel, reubicar paneles y colocar optimizadores
> - `FAQ Suntropy (1).pdf` - Confirmacion de que se usan las dimensiones reales de los paneles para calcular sombras entre filas
