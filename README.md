# Base de Conocimiento Suntropy

Repositorio de documentacion para el asistente de soporte de Suntropy. Organizado por dominio para facilitar la busqueda por herramientas cat, grep y busqueda semantica.

## Estructura

- `faqs.md` - Preguntas frecuentes con enlaces [[wikilinks]] a documentos de conocimiento
- `estudios/` - Documentacion sobre los tipos de estudios y sus funcionalidades
- `configuracion/` - Configuracion de la plataforma, inventario, plugins, usuarios
- `plantillas/` - Editor de plantillas de presupuesto y personalizacion
- `licencias/` - Creditos, suscripciones y metodos de pago
- `soporte/` - Canales de ayuda y recursos de formacion
- `connect/` - Suntropy Connect: el programa de escritorio que conecta PVsyst y PV*SOL con Claude o ChatGPT

## PDFs complementarios

Los documentos markdown contienen la informacion estructurada y organizada. Para ampliar detalles, cada documento indica que PDFs consultar via busqueda semantica. Los PDFs disponibles son transcripciones del Crash Course de Suntropy (videos de YouTube):

| PDF | Contenido |
|-----|-----------|
| `Configuracion (2).pdf` | Menu, inventario, documentos, perfil de usuario, plugins, configuracion predeterminada |
| `Autoconsumo Individual (1).pdf` | Los 6 pasos del estudio de autoconsumo individual |
| `Autoconsumo Colectivo (3).pdf` | Perfiles, consumo agregado, superficies, coeficientes de reparto, balance, compartir |
| `Aerotermia (2).pdf` | Los 4 pasos del estudio de aerotermia |
| `Punto de Recarg vehiculo electrico (1).pdf` | Estudio de punto de recarga y 3 formas de incluirlo |
| `Plantillas (1).pdf` | Editor de plantillas: tema, componentes, texto parametrico, condicionales, equipos personalizados |
| `FAQ Suntropy (1).pdf` | Preguntas frecuentes tecnicas originales |
| `Calculo de baterias.pdf` | Documento tecnico del algoritmo de calculo de baterias |

## Como buscar informacion

1. **grep/busqueda por keywords**: Los nombres de archivo y titulos H1 contienen los terminos clave de cada tema
2. **cat**: Cada documento es atomico (un concepto por fichero), se puede leer completo para obtener toda la info
3. **Busqueda semantica**: Los wikilinks [[]] conectan documentos relacionados. Si encuentras un doc, los wikilinks te guian a docs complementarios
4. **Busqueda en PDFs**: Cada doc indica que PDFs consultar para informacion ampliada (transcripciones de videos con explicaciones paso a paso)

## Aviso sobre la sincronizacion con Devic

Este repositorio **no se sincroniza solo** con la base de conocimiento de Devic. La
importacion inicial fue manual (marzo de 2026) y desde entonces se han editado documentos
directamente en Devic: a fecha de septiembre de 2026 alli hay tres documentos que aqui no
estan (`licencias/planes-de-suscripcion`, `configuracion/Configuracion de Precio en Baterias
Modulares`, `estudios/Incluir impuestos en precios de energia`) y `faqs.md` va por la sexta
version.

Consecuencia practica: **no vuelques este repo sobre Devic dando por hecho que es la fuente
de verdad**, porque se perderia ese trabajo. Un cambio aqui hay que llevarlo tambien a Devic
(`devic documents create|update`), que es lo que el asistente lee de verdad.
