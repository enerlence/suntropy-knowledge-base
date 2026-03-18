# Inventario

El inventario es el primer elemento que hay que configurar para comenzar a trabajar con Suntropy. Se accede desde **Herramientas > Inventario**.

## Tipos de equipos

### Paneles solares
Campos: potencia (Wp), eficiencia (%), fabricante, modelo, dimensiones (ancho x alto), precio.

### Inversores
Campos: potencia nominal (W), tipo (monofasico/trifasico), fabricante, modelo, precio.

### Baterias
Campos: capacidad (kWh), profundidad de descarga (%), eficiencia (%), fabricante, modelo, precio. Ver [[baterias-y-optimizacion]] para detalles del calculo.

### Aerotermias
Equipos de aerotermia con sus especificaciones tecnicas. Se usan en los [[estudio-aerotermia|estudios de aerotermia]].

### Puntos de recarga
Cargadores para vehiculo electrico. Se usan en los [[punto-de-recarga|estudios de punto de recarga]].

## Kits solares

Para crear kits:
1. Primero tener cargados los paneles e inversores
2. Crear el kit seleccionando la cantidad y tipo de paneles y el inversor asociado
3. Definir si el kit es [[kits-coplanares|coplanar o no coplanar]]

## Carga masiva

Si se tiene un gran volumen de equipos, el equipo de Suntropy puede proporcionar un archivo plantilla para cargar equipos en bloque.

## Desactivar equipos

Los equipos que ya no se usen se pueden **desactivar** (sin eliminarlos) para que no aparezcan en los estudios. Esto es preferible a eliminarlos para mantener el historico.

## Equipos personalizados

Ver [[equipos-personalizados]] para crear categorias de equipos adicionales (cableado, estructuras, mano de obra, etc.).

## Busqueda y filtrado

Se puede buscar equipos por marca directamente en el inventario (ej. escribir "Canadian" para filtrar paneles de esa marca).

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `Configuracion (2).pdf` - Video "Configura tu inventario (Paso 2)" con demostracion practica de como cargar paneles, inversores, baterias, aerotermias y puntos de recarga. Muestra como crear kits solares, buscar por marca y la opcion de carga masiva con plantilla
> - `Configuracion (2).pdf` - Video "Domina todos los Plugins de Suntropy" donde se explica la relacion entre equipos personalizados, presupuesto avanzado y plantillas de presupuesto
