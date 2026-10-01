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

### Hay permanencia? Puedo contratar Suntropy solo algunos meses?

No hay permanencia. Se puede contratar un mes y darse de baja en cuanto se quiera, y volver a contratar mas adelante (por ejemplo, solo los meses en los que se hacen estudios): la cuenta no se borra al bajar al plan gratuito. Pagar un año por adelantado es opcional y tiene un **20 % de descuento** sobre el precio mensual.

Mas informacion: [[planes-de-suscripcion]], [[suscripcion-y-pagos]]

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

### Suntropy se conecta con SIPS para obtener los consumos?

No. Por normativa, el acceso al SIPS es para fines de facturacion de las comercializadoras, no para uso comercial. Para tener la curva real del cliente, Suntropy se integra con **Datadis** (con el consumidor autorizado y la cuenta conectada). Tambien se puede importar un Excel de consumos, y Alexandria lo convierte al formato de Suntropy aunque venga en otro formato.

Mas informacion: [[curvas-de-consumo]], [[integraciones]]

### Se puede ver que parte del ahorro corresponde a las baterias?

Si. En un estudio con almacenamiento se pueden mostrar los resultados **con y sin bateria** dentro del mismo estudio para comparar ahorro y rentabilidad. El calculo de baterias es horario para todo el ano, con una estrategia de carga y descarga simplificada (sin optimizacion de despacho).

Mas informacion: [[baterias-y-optimizacion]]

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

## Suntropy AI y Alexandria

### Que es Suntropy AI y que es Alexandria?

Suntropy AI es el Suntropy de siempre con una compañera de inteligencia artificial: **Alexandria**. Alexandria es un agente de IA que conoce Suntropy y el sector de la energia renovable: hace estudios, gestiona el inventario, edita plantillas y presupuestos, prepara legalizaciones y trabaja con las apps del negocio (correo, Google Drive, CRM). Esta en la seccion **Alexandria** del menu superior y en la pestaña flotante del borde derecho (**⌘J / Ctrl+J**).

Mas informacion: [[que-es-suntropy-ai]]

### En que se diferencia Alexandria de ChatGPT o Claude?

Funciona con modelos de ese tipo, pero esta **entrenada y documentada para los procesos del sector** (estudios en Suntropy, facturas electricas, legalizaciones) y consulta una **base de conocimiento verificada** (IDAE, reales decretos, guias de tramitacion, manuales tecnicos) en lugar de depender de lo que encuentre en Internet. Llega antes al resultado y con menos errores, y ademas opera dentro de Suntropy.

Mas informacion: [[que-es-suntropy-ai]]

### Que puedo pedirle a Alexandria?

Algunos ejemplos: dar de alta un panel o inversor desde su ficha tecnica (o buscandola en Internet); hacer un estudio de autoconsumo desde cero, desde una factura o desde un Excel de consumos; añadir paginas a un presupuesto o diseñar una plantilla; consultar normativa y subvenciones; preparar la documentacion de legalizacion; guardar documentos en Google Drive o enviarlos por correo. Puede trabajar en segundo plano y con varias tareas a la vez.

Mas informacion: [[que-puede-hacer-alexandria]]

### Hacer un estudio con Alexandria consume creditos?

Si. Crear un estudio consume los mismos **creditos de Suntropy (soles)** que si lo creara el usuario. Por eso Alexandria pide confirmacion antes de crearlo. El uso de Alexandria (su plan) es aparte y no incluye creditos de estudios.

Mas informacion: [[creditos]], [[planes-de-alexandria]]

### Alexandria puede dibujar la cubierta?

Todavia no: navega hasta la direccion y pide al usuario que dibuje la superficie; despues continua sola. Cuando se le pide el estudio por correo, en lugar de dibujar la cubierta optimiza directamente la potencia pico.

Mas informacion: [[que-puede-hacer-alexandria]]

### Como hago que no me pida confirmacion en cada paso?

Diciendoselo: por ejemplo, "recuerda no pedirme autorizacion en los pasos intermedios". Lo guarda en su memoria y deja de preguntar. Las confirmaciones existen por seguridad y para no consumir creditos sin autorizacion.

Mas informacion: [[canales-e-integraciones-alexandria]]

### Puedo hablarle en lugar de escribir?

Si, de dos formas: con **mensajes de voz**, que transcribe automaticamente, o con una **conversacion de voz en tiempo real**. Hablarle por WhatsApp o por llamada esta en desarrollo.

Mas informacion: [[canales-e-integraciones-alexandria]]

### Puedo escribirle por correo electronico?

Si, a **alexandria@suntropy.ai**. Se le pueden pedir dudas, revisiones de estudios o datos de las apps conectadas, y adjuntarle una factura y un Excel de consumos para que haga practicamente todo el estudio.

Mas informacion: [[canales-e-integraciones-alexandria]]

### Alexandria recuerda cosas? Puedo ver o borrar lo que recuerda?

Si. Guarda **recuerdos** (preferencias, datos de la empresa, forma de trabajar) y los usa en las siguientes conversaciones. Se ven y se pueden editar desde el inicio de la seccion Alexandria. En el onboarding se le pueden subir tres o cuatro presupuestos propios para que aprenda el estilo de la empresa.

Mas informacion: [[canales-e-integraciones-alexandria]]

### Alexandria puede hacer la legalizacion de una instalacion?

Si. A partir de un estudio prepara la documentacion con los **modelos oficiales de la comunidad autonoma** (PDF rellenables, Word, Excel) y el **diagrama unifilar**. Tiene recetas para las 17 comunidades autonomas y Ceuta y Melilla. Son borradores que debe revisar y firmar el instalador habilitado.

Mas informacion: [[legalizaciones-con-alexandria]]

### Con que aplicaciones se conecta Alexandria?

Desde el panel de aplicaciones conectadas de Alexandria: por ejemplo Gmail, Google Drive y HubSpot, y se iran añadiendo mas (tambien del sector). Se pulsa **Conectar** y se autoriza en el navegador. Los usuarios avanzados pueden añadir **su propio MCP** (un conector estandar para agentes de IA). La conexion con PVsyst y PV\*SOL se hace con [[que-es-suntropy-connect|Suntropy Connect]].

Mas informacion: [[canales-e-integraciones-alexandria]]

### Cuanto cuesta Alexandria?

Toda cuenta de Suntropy tiene un **uso incluido** gratis. Para ampliarlo hay tres planes por cuenta y mes, sin IVA: **Pro** 19,99 € (x2 el uso incluido), **Max** 90 € (x6) y **Ultra** 200 € (x15). Se solicitan en **Configuracion > Plan > Alexandria** y los activa el equipo de Suntropy.

Mas informacion: [[planes-de-alexandria]]

### Necesito un plan de pago de Suntropy para usar Alexandria?

No. Los planes de Alexandria son independientes de los de Suntropy: cualquier cuenta, tambien la gratuita, tiene el uso incluido y puede contratar un plan de Alexandria sin tener un plan de pago de estudios.

Mas informacion: [[planes-de-alexandria]]

### El uso de Alexandria es por usuario o por empresa?

Por empresa: el plan es de toda la cuenta y lo comparten sus usuarios. Para que nadie agote el de todos hay un **limite mensual de la cuenta** y un **limite diario por usuario**. Cuando se alcanza uno, el chat avisa de cuando vuelve a estar disponible; se puede esperar o ampliar el plan.

Mas informacion: [[planes-de-alexandria]]

---

## LeadGen

### Que es LeadGen?

Una herramienta de Suntropy AI para crear **campañas automatizadas que encuentran y cualifican empresas** que pueden ser clientes de energia solar: autoconsumo industrial, baterias o mantenimiento para quien ya tiene placas, autoconsumo colectivo… De cada lead puede obtener la cubierta y su superficie, si ya tiene placas (con año aproximado y potencia estimada), el consumo estimado, la facturacion y el LinkedIn de la empresa y del decisor. Los resultados se ven en tabla y mapa y se exportan a Excel.

Mas informacion: [[leadgen]]

### Sirve para encontrar particulares?

No: esta pensado para **B2B**. Sus fuentes son Google Maps y datos abiertos, asi que encuentra empresas.

Mas informacion: [[leadgen]]

### Cuanto cuesta LeadGen y como lo pruebo?

Funciona con **creditos de LeadGen**: **5 € por cada 1.000 creditos**. El coste por lead depende de los pasos elegidos y de la zona (por ejemplo, unos 39 creditos, 0,19 €, por lead cualificado con consumo, CIF y deteccion de placas). Quien se inscriba en https://www.suntropy.ai/leadgen/ tiene **acceso anticipado desde el 5 de octubre de 2026 con 2.000 creditos de regalo**; el lanzamiento abierto es el 20 de octubre de 2026. La pagina tiene una calculadora para estimar el coste de una campaña.

Mas informacion: [[leadgen]]

### Los creditos de LeadGen son los mismos que los de Suntropy?

No. Los creditos de Suntropy (soles) sirven para crear estudios de autoconsumo; los de LeadGen, para las campañas de captacion. Son independientes, se compran por separado y tampoco forman parte de los planes de Alexandria.

Mas informacion: [[leadgen]], [[creditos]]

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
