# Preguntas Frecuentes (FAQs) de Suntropy

Documento de preguntas frecuentes del soporte de Suntropy. Cada respuesta enlaza a documentos de conocimiento detallados para ampliar informacion.

---

## Licencias y creditos

### Los creditos de Suntropy, son acumulables?

No, los creditos no son acumulativos. Existen dos tipos: **Creditos Normales** (se reinician al inicio del mes) y **Creditos Bonus** (se mantienen hasta usarse). Los creditos se consumen al crear estudios, no al actualizarlos. El sistema consume primero los Bonus y luego los Normales.

Mas informacion: [[creditos]]

### Que metodos de pago puedo usar y como gestionar mi suscripcion?

Suntropy utiliza Stripe como plataforma de pago. Se puede cambiar a plan Freemium en cualquier momento (con restricciones). Para problemas con pagos, contactar con soporte@suntropy.es.

Mas informacion: [[suscripcion-y-pagos]]

---

## Configuracion

### Como configurar el inventario en Suntropy?

Ve a **Herramientas > Inventario**. Es lo primero que hay que configurar. Se pueden anadir paneles, inversores, baterias, aerotermias y puntos de recarga de forma individual. Para crear kits solares, primero cargar paneles e inversores. Los equipos en desuso se pueden desactivar sin eliminarlos. Para carga masiva, el equipo de Suntropy puede proporcionar una plantilla.

Mas informacion: [[inventario]]

### Si eliminamos un panel, desaparece de los estudios en los que se ha utilizado?

No. Al crear un estudio, Suntropy guarda una **copia de los datos del panel** dentro del propio estudio, no una referencia al inventario. Por eso, si se elimina (o se desactiva) un panel del inventario, **los estudios donde ya se uso siguen intactos**: conservan las caracteristicas del panel original y se pueden seguir consultando, editando y exportando. Lo unico que cambia es que ese panel deja de estar disponible para nuevos estudios. Si el equipo va a dejar de usarse pero quieres mantener trazabilidad clara en el inventario, lo recomendable es **desactivarlo** en lugar de eliminarlo.

Mas informacion: [[inventario]]

### Que plugins estan disponibles en Suntropy?

Los plugins se activan en **Configuracion > Plugins**. Incluyen: complementos de consumo, equipos personalizados, presupuesto avanzado, recomendacion de inversor, trasladar consumo, intervalos de potencia, control de versiones, imagenes externas, IVA reducido, chat en presupuestos, entre otros.

Mas informacion: [[plugins]]

### Que es el plugin de equipos personalizados?

Permite crear categorias de equipos adicionales en el inventario (cableado, estructuras, mano de obra, etc.). Se configuran con campos personalizados y pueden tener cantidad proporcional al numero de paneles. Aparecen como partidas adicionales en el balance economico.

Mas informacion: [[equipos-personalizados]]

### Que es el plugin de intervalos de potencia?

Permite crear rangos de precios escalonados basados en un ratio euros/Wp. Se configuran plantillas con rangos de potencia y en el balance economico se aplica automaticamente el ratio correspondiente.

Mas informacion: [[intervalos-potencia]]

### Que roles de usuario existen en Suntropy?

Tres roles: **Administrador** (acceso total), **Tecnico** (crear/editar estudios, sin acceso a configuracion) y **Comercial** (solo generar PDFs). Se gestionan en Configuracion > Usuarios.

Mas informacion: [[usuarios-y-roles]]

### Como cambiar mis credenciales de acceso a Suntropy?

Ve a **Configuracion > Perfil de usuario > Editar**. Desde ahi se puede cambiar correo electronico y contrasena. Tambien se puede cambiar moneda e idioma.

Mas informacion: [[credenciales-y-perfil]]

### Que es el modo Demo?

Permite probar Suntropy con kits y paneles predefinidos sin configurar inventario. Los datos del modo Demo no se conservan al desactivarlo. Se activa desde la barra superior.

Mas informacion: [[modo-demo]]

### Que integraciones estan disponibles en Suntropy?

Datadis (curvas de consumo), SMTP personalizado, CRM (Odoo, Zoho, HubSpot via webhooks/Akiki), firma digital, Pontio (financiacion) y calculadora solar embebible.

Mas informacion: [[integraciones]]

### Para que sirven los estados de los estudios?

Permiten clasificar el ciclo de vida del estudio (Creado, Enviado, Aceptado, Cerrado). Se pueden crear nuevos estados con nombre y color. No se pueden eliminar, solo desactivar.

Mas informacion: [[estados-estudios]]

---

## Estudios solares - Autoconsumo individual

### Como introducir una curva de consumo en un estudio solar?

Cuatro metodos: **Patrones de consumo** (~90% de usuarios, integrado con REE), **Facturas** (manual por periodos), **Importar CSV/Excel** (necesario para tarifas 6.X TD), y **Datadis** (importacion directa). Se pueden anadir complementos de consumo (coche electrico, aire acondicionado) y trasladar consumo.

Mas informacion: [[curvas-de-consumo]]

### Como anadir una curva de carga en Excel?

En el paso 2 del estudio, seleccionar "Importar curva de consumo", descargar la plantilla, rellenar datos horarios, establecer fechas y cargar el archivo. Necesario para tarifas 6.X TD.

Mas informacion: [[curvas-de-consumo]]

### Como se calculan las curvas de carga y por que se usan los perfiles de REE?

Se usan los perfilados de Red Electrica Espanola (REE) porque no es comun disponer de una curva horaria real. REE distribuye el consumo total segun tarifa ATR y zona geografica. No disponible para tarifas 6.X TD.

Mas informacion: [[curvas-de-consumo]]

### De donde se obtienen los datos de produccion solar?

De **PVGIS** (Comision Europea). Usa coordenadas geograficas, orientacion (azimut), inclinacion y perdidas del sistema para calcular la produccion horaria. Tambien puede optimizar orientacion e inclinacion.

Mas informacion: [[produccion-solar-pvgis]]

### Como se muestran los datos de produccion por periodos?

Desglosados en hasta 6 periodos tarifarios (P1-P6) con agregacion mensual. Se muestran en el paso 5 (Resultados) con vistas de produccion total, por superficie, Inspector y descarga en Excel.

Mas informacion: [[produccion-solar-pvgis]]

### Como funciona la optimizacion de potencia?

Desde el kit de mayor potencia que cabe en la superficie, itera reduciendo paneles hasta cumplir el criterio seleccionado. Cinco modos: meses con excedentes, porcentaje de excedentes, ahorro energetico, ahorro economico y porcentaje de consumo total.

Mas informacion: [[optimizacion-potencia]]

### Se tienen en cuenta las sombras entre paneles?

Si. Sombras entre filas de paneles se calculan automaticamente. Sombras de obstaculos se pueden dibujar, asignar altura, ejecutar analisis y visualizar con escala de colores. Permite reubicar paneles, colocar optimizadores o eliminar los mas sombreados.

Mas informacion: [[sombras-y-obstaculos]]

### Por que el retorno de inversion (anos) es alto?

Posibles causas: sobredimensionamiento, modalidad de inyeccion 0, bajos precios de energia, mala orientacion, bajo autoconsumo, sin subvenciones. Verificar precios de energia y modalidad de excedentes.

Mas informacion: [[roi-retorno-inversion]]

### Que modalidades de retribucion de excedentes existen?

Cuatro modalidades: **Vertido a red** (venta al precio fijado en euros/MWh), **PPA** (descuento del precio de la instalacion), **Inyeccion 0** (sin excedentes en calculo) y **Bateria virtual** (monedero virtual). Se selecciona en el paso 6.

Mas informacion: [[excedentes-y-retribucion]]

### Cuales son los criterios de optimizacion de baterias?

Tres criterios: excedentes totales almacenables (%), porcentaje de autoconsumo (independencia energetica) y dias de autonomia. El sistema evalua las baterias del inventario y filtra las que cumplen los criterios.

Mas informacion: [[baterias-y-optimizacion]]

### Para que sirven los precios alternativos de potencia y energia?

Se usan cuando se quiere ofertar un cambio de tarifa electrica ademas de la instalacion solar. Suntropy calcula el ahorro combinado: beneficio solar + optimizacion del contrato electrico.

Mas informacion: [[precios-alternativos]]

### Puedo guardar un estudio incompleto?

Si, se puede guardar en cualquier momento pulsando "Guardar". El estudio aparece en el dashboard con el indicador de progreso (ej. 3/6).

Mas informacion: [[guardar-estudio-incompleto]]

### Que diferencia hay entre kits coplanares y no coplanares?

Kits coplanares: superficies sin inclinacion de paneles (paralelos a cubierta). Kits no coplanares: superficies con inclinacion definida (estructura con angulo). La seleccion se filtra automaticamente segun la superficie.

Mas informacion: [[kits-coplanares]]

---

## Estudios - Aerotermia

### Como seleccionar aerotermia en un estudio?

Seleccionar "Estudio Aerotermia" en el selector de tipo de estudio. El estudio tiene 4 pasos: datos del cliente, seleccion de aerotermia (calcula potencia recomendada), calculo de ahorros (sustitucion de combustible) y balance economico.

Mas informacion: [[estudio-aerotermia]]

### Como anadir datos de cliente en un estudio de aerotermia?

En el paso 1: nombre, provincia, tarifa de acceso y precios de energia por periodos. Al completar los campos obligatorios se habilita la flecha verde para continuar.

Mas informacion: [[estudio-aerotermia]]

---

## Estudios - Autoconsumo colectivo

### Como funciona el autoconsumo colectivo en Suntropy?

Permite dimensionar instalaciones compartidas. Se introducen consumidores agrupados en perfiles, se genera la curva agregada, se selecciona superficie (radio max 2 km), se eligen coeficientes de reparto (equitativo, proporcional, personalizado) y se genera un enlace unico para que cada participante vea sus resultados.

Mas informacion: [[autoconsumo-colectivo]]

---

## Estudios - Punto de recarga

### Como hacer un estudio de punto de recarga para vehiculo electrico?

Tres opciones: estudio independiente (3 pasos), como complemento de consumo en estudio de autoconsumo (plugin), o como equipo personalizado en el balance economico.

Mas informacion: [[punto-de-recarga]]

---

## Plantillas

### Como modificar plantillas de presupuesto?

En **Herramientas > Plantillas**. El editor permite: modificar tema (colores, logo), anadir componentes (graficas, KPIs, textos parametricos, imagenes), fondos de pagina, configuracion condicional (por financiacion, bateria, tarifa), y duplicar/eliminar componentes. Guardar frecuentemente.

Mas informacion: [[editor-de-plantillas]]

---

## Documentos

### Que hay en la seccion de Documentos?

En **Herramientas > Documentos**: estudios compartidos (con metricas de visualizacion), plantillas, fondos de pagina y firmas digitales (documentos enviados a firmar con estado).

Mas informacion: [[gestion-documentos]]

---

## Suntropy Connect (PVsyst y PV*SOL)

### Que es Suntropy Connect?

Un programa de escritorio para Windows que conecta el **PVsyst** o el **PV\*SOL** ya instalados en el ordenador con un asistente de IA (Claude o ChatGPT), para pedirle en lenguaje natural que simule, compare variantes o resuma resultados. La licencia, el ordenador y los proyectos se quedan donde estan. Se descarga en https://connect.suntropy.ai

Mas informacion: [[que-es-suntropy-connect]]

### Puedo simular en PV*SOL desde Suntropy Connect?

No, y no es algo pendiente: PV\*SOL no tiene linea de comandos ni API de calculo. Lo que si hace es **leer los resultados que el proyecto ya lleva guardados dentro**, que en PV\*SOL es mucho: produccion, autoconsumo, excedentes, cobertura solar, PR y la cascada de perdidas. En PVsyst si se simula, se crean y se editan proyectos.

Mas informacion: [[que-es-suntropy-connect]]

### Como vinculo mi ordenador?

Se instala `PVsystConnect-Setup.exe` en el equipo que tiene PVsyst o PV\*SOL, se abre, y el programa muestra un codigo de emparejamiento que se aprueba en la pantalla `/link-device` de Suntropy. El codigo **caduca a los 10 minutos**; si se pasa, el programa da uno nuevo.

Mas informacion: [[instalacion-y-vinculacion-connect]]

### Me he registrado y no tengo ningun codigo

El codigo lo da el programa de escritorio: hasta instalarlo no hay ninguno que escribir. La pantalla `/link-device` ofrece la descarga justo debajo del campo del codigo.

Mas informacion: [[instalacion-y-vinculacion-connect]]

### Cuanto cuesta y hay prueba gratuita?

Prueba de **7 dias sin tarjeta**, y despues plan Individual a **18 EUR/mes** por usuario con pago anual (22,50 EUR/mes pagando mes a mes). La prueba es **una por empresa**, no una por usuario: si un companero ya la activo, esa cuenta la tiene consumida.

Mas informacion: [[licencia-y-prueba-connect]]

### Suntropy Connect incluye la licencia de PVsyst?

No. Simular (`run_simulation`, `run_batch`) consume cuota de la **licencia de PVsystCLI del usuario**, que se contrata con PVsyst. Leer resultados, hacer graficas y crear o editar proyectos no consumen nada, y ninguna consulta de PV\*SOL consume licencia.

Mas informacion: [[licencia-y-prueba-connect]]

### Cuantas personas pueden usarlo a la vez?

Las que permitan las **plazas** de la licencia, una por usuario. Un mismo usuario en dos ordenadores se desplaza a si mismo; si no quedan plazas, quien entra desaloja al menos activo.

Mas informacion: [[licencia-y-prueba-connect]]

### Como desconecto un ordenador?

En **Configuracion > Integraciones > Suntropy Connect**. Desconectar **no cancela** la suscripcion: ese mismo equipo puede volver a conectarse cuando haga falta.

Mas informacion: [[gestion-de-equipos-connect]]

---

## Soporte

### Donde puedo encontrar ayuda y soporte de Suntropy?

Email (soporte@suntropy.es), chat de soporte en la plataforma, canal de YouTube "Suntropy AI" con Crash Course modular, y curso online en https://suntropy.es/curso-intensivo.

Mas informacion: [[canales-de-ayuda]]
