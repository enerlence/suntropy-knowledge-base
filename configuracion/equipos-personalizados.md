# Equipos Personalizados

El plugin de Equipos Personalizados permite crear categorias de equipos adicionales dentro del [[inventario]] que no son paneles, inversores ni baterias. Ejemplos: cableado, estructuras, mano de obra, protecciones, packs residenciales, etc.

## Como configurar

1. Activar el plugin en **Configuracion > [[plugins|Plugins]]**
2. Ir a **Inventario > Equipos Personalizados**
3. Hacer clic en **"Crear equipo personalizado"**
4. Introducir el nombre de la categoria (ej. "Estructuras")
5. Definir las columnas/campos que tendra (nombre, tipo, dimensiones, precio, etc.)

### Opciones importantes

- **Cantidad proporcional al numero de paneles**: Si se activa, las unidades se calculan automaticamente segun el numero de paneles del estudio
- **Pertenece a la partida de materiales**: Para que se incluya en el calculo del presupuesto avanzado

6. Anadir los equipos individuales dentro de cada categoria

## Uso en estudios

En el paso 6 (Balance Economico) del [[autoconsumo-individual|estudio de autoconsumo]], los equipos personalizados aparecen como partidas adicionales que se suman al precio de paneles, inversores y baterias.

## Uso en plantillas

Se pueden anadir los equipos personalizados a las [[editor-de-plantillas|plantillas de presupuesto]] usando:
- El componente **"Texto parametrico"** con las formulas de equipos personalizados
- El componente **"Imagen de equipo personalizado"**

## ID de referencia

Los equipos personalizados pueden tener un **ID de referencia** para empresas que tienen integracion con un CRM (Odoo, etc.) para que Suntropy identifique que equipo corresponde en el sistema externo.

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `Configuracion (2).pdf` - Video "Domina todos los Plugins de Suntropy" con demostracion de como crear categorias de equipos personalizados (ejemplo: "Estructuras"), definir columnas (nombre, tipo, dimensiones, precio), activar cantidad proporcional a paneles, y como aparecen en el balance economico
> - `Plantillas (1).pdf` - Video "Anade los Equipos Personalizados a la plantilla" con demostracion de como usar texto parametrico con formulas de equipos personalizados e imagen de equipo personalizado en plantillas
