# Qué puede hacer Alexandria

Los casos de uso, de lo más sencillo a lo más complejo. En todos, Alexandria **puede trabajar
en segundo plano**: se le encarga la tarea y se puede seguir con otra cosa, o lanzar varias
conversaciones a la vez.

## Inventario

- **Dar de alta equipos desde la ficha técnica.** Se le adjunta el PDF (paneles, inversores,
  baterías…), extrae los datos, propone el equipo y lo crea tras confirmarlo. Ver
  [[inventario]].
- **Sin ficha técnica**: puede buscar el modelo en Internet ("un panel de la misma marca pero
  de 550 W") y crearlo igual.
- **Revisar el inventario**: por ejemplo, cruzar los últimos estudios con los paneles del
  inventario para ver cuáles hace tiempo que no se usan.

## Estudios de autoconsumo

- **Desde cero**, con los datos básicos: cliente, CUPS, dirección o coordenadas (las convierte
  y sitúa el punto en el mapa) y consumo. Alexandria abre el estudio y lo va completando paso a
  paso: datos, consumo, producción (con [[produccion-solar-pvgis|PVGIS]], como siempre),
  resultados y presupuesto. Ver [[autoconsumo-individual]].
- **Desde una factura**: se le adjunta la factura y extrae titular, potencia contratada,
  consumos y precios. Sabe leer los distintos formatos de factura y detectar datos que no
  cuadran.
- **Desde un Excel de consumos** en cualquier formato: lo convierte al formato que necesita
  Suntropy, sin tener que adaptarlo a mano. Ver [[curvas-de-consumo]].
- **Con baterías**: se le puede pedir que añada almacenamiento y calcule el estudio con
  baterías. Ver [[baterias-y-optimizacion]].
- **Con curvas reales de Datadis**, si el consumidor está autorizado y la cuenta de Datadis
  está conectada. Ver [[integraciones]].

Lo que conviene saber:

- **La cubierta la dibuja el usuario.** Alexandria navega hasta la dirección y pide dibujar la
  superficie; dibujarla ella sola está en desarrollo. Cuando se pide el estudio por correo, en
  lugar de dibujar optimiza la potencia pico directamente.
- **Pide confirmación en los pasos sensibles**: precios de la energía, tarifa de acceso,
  coste de la instalación y, sobre todo, antes de crear el estudio, porque **crear un estudio
  consume créditos (soles) de Suntropy** igual que si lo hiciera el usuario. Ver [[creditos]].
  Si no se quieren confirmaciones intermedias, basta con decírselo ("recuerda no pedirme
  autorización en los pasos intermedios") y lo apunta en su memoria.

## Plantillas y presupuestos

- **Añadir páginas a un presupuesto concreto**: "añade después del análisis de consumo una
  página con el cálculo de la producción y la comparación mes a mes". Se puede iterar (añadir
  una gráfica, una tabla…) y, al guardar, el cambio afecta **sólo a ese documento**, no a la
  plantilla.
- **Incluir material externo**: capturas, curvas exportadas de PVsyst o PV\*SOL, análisis de
  sombras… para clientes que piden una propuesta más técnica.
- **Editar o diseñar plantillas** enteras, o varias con distintos formatos. Lo más práctico es
  partir de una de las **plantillas predefinidas** (las cuentas gratuitas tienen tres; el
  catálogo completo depende del plan) y pedirle que la adapte. Ver [[editor-de-plantillas]].

## Información del sector

Responde con fuentes verificadas sobre normativa, tramitación, autoconsumo colectivo,
subvenciones, etc. Durante un estudio se le puede preguntar, por ejemplo, qué ayudas hay en esa
comunidad autónoma o provincia, y que además busque en Internet convocatorias adicionales.

## Legalizaciones

Prepara la documentación de legalización de una instalación de autoconsumo con los modelos
oficiales de la comunidad autónoma. Tiene su propio documento:
[[legalizaciones-con-alexandria]].

## Trabajar con otras apps

Con las apps conectadas puede, por ejemplo, guardar los documentos generados en una carpeta de
Google Drive o mandarlos por correo desde tu Gmail. Ver
[[canales-e-integraciones-alexandria]].

## Captación de clientes

Con [[leadgen|LeadGen]], Alexandria monta campañas para encontrar y cualificar empresas que
puedan ser clientes.

## Documentos relacionados

- [[que-es-suntropy-ai|Qué es Suntropy AI]]
- [[canales-e-integraciones-alexandria|Canales, memoria e integraciones]]
- [[planes-de-alexandria|Planes y uso de Alexandria]]
