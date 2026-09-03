# Problemas frecuentes de Suntropy Connect

Los casos que de verdad aparecen, con lo que hay que hacer en cada uno.

## Al vincular el ordenador

### "El código ha caducado"

Los códigos de emparejamiento **duran 10 minutos**. Pasado ese rato dejan de valer, y es lo
normal si la persona se ha entretenido creando la cuenta o validando el correo.

No hay nada que arreglar: se vuelve al programa de escritorio, que muestra un código nuevo, y
se escribe en `/link-device`. La pantalla tiene un botón **"Escribir otro código"** para no
tener que recargarla.

### "Código no válido" o "no encontramos ese código"

Casi siempre es un error al teclear —conviene repasar los ocho caracteres— o un código que ya
se aprobó antes. Si el ordenador ya aparece en
[[gestion-de-equipos-connect|Configuración → Integraciones]], está vinculado y no hace falta
volver a aprobarlo.

### Entré a iniciar sesión y acabé en la página de inicio

Era un fallo real y **está corregido**: el destino sobrevive al login, incluso cuando el
inicio de sesión salta de un dominio a otro. Si aún así ocurre —por ejemplo con un enlace
antiguo guardado—, la salida es entrar en Suntropy y volver a `/link-device`, donde se puede
escribir el código a mano.

### Me he registrado pero no tengo ningún código

**El código lo da el programa de escritorio.** Quien llega desde la web de Connect y crea la
cuenta antes de instalar nada no tiene todavía ningún código que escribir. La pantalla de
`/link-device` ofrece la descarga justo debajo del campo. Ver
[[instalacion-y-vinculacion-connect]].

### "Esta cuenta no tiene una licencia de Suntropy Connect en vigor"

La vinculación está bien; lo que falta es la licencia. Desde la misma pantalla de
`/link-device` se puede **activar la prueba de 7 días** y seguir sin salir de ahí. Si el
botón dice que no se puede, es que **la prueba de esa empresa ya está consumida**: la licencia
es de la cuenta, no de la persona. En ese caso hay que contratar en
[[licencia-y-prueba-connect|`/pvsyst-plan`]].

### El programa no encuentra mi PVsyst

Detecta las instalaciones de **PVsyst 8.x** en las rutas habituales. Si está en otro sitio o
es una versión anterior, no lo verá. Para PV\*SOL, si falta alguna carpeta de proyectos se
puede añadir a mano desde el programa.

## Al usarlo desde Claude o ChatGPT

### El asistente no ve las herramientas

El conector se activa **por conversación**: hay que encenderlo en el menú «+» de Claude o en
el de plugins de ChatGPT, en esa conversación concreta. Y comprobar que la dirección dada de
alta es la del motor correcto —`/pvsyst/mcp` o `/pvsol/mcp`—, que son dos
[[conectar-claude-y-chatgpt|conectores distintos]].

### Se me desconecta solo cuando trabaja un compañero

Es el reparto de **plazas**. Si la licencia tiene menos plazas que gente conectada, quien
entra desaloja al menos activo. Y una misma persona en dos ordenadores se desplaza a sí
misma: una persona, una plaza. Con volver a conectar desde el programa se recupera. Ver
[[licencia-y-prueba-connect|el detalle de las plazas]].

### PVsyst dice que no quedan ejecuciones

Es la **cuota de la licencia de PVsystCLI**, que es del usuario y no va incluida en la
suscripción de Suntropy Connect. Sólo la gastan `run_simulation` y `run_batch`; leer
resultados, hacer gráficas y editar proyectos no cuestan nada.

Truco: un **barrido en modo batch cuesta una sola llamada**, lleve los casos que lleve. Pedir
un barrido gasta mucho menos que lanzar las simulaciones una a una.

### De un proyecto de PV\*SOL no salen resultados

Lo más probable es que **ese proyecto no se haya simulado nunca**. PV\*SOL guarda los
resultados dentro del propio fichero, y Connect no puede simular en PV\*SOL: si el `.pvprj` no
los lleva dentro, no hay número que dar. Hay que abrirlo en PV\*SOL, simularlo y guardarlo.

### Los datos de PV\*SOL vienen por meses y yo quería por horas

Es así por diseño: en PV\*SOL la resolución es **mensual**, doce valores por magnitud, y no hay
variantes. Las series horarias y el CSV son cosa de PVsyst. Ver
[[que-es-suntropy-connect|los dos motores]].

## Si nada de esto encaja

Escribir a soporte@suntropy.es o usar el chat de soporte de la plataforma. Ver
[[canales-de-ayuda]].

## Documentos relacionados

- [[que-es-suntropy-connect|Qué es Suntropy Connect]]
- [[instalacion-y-vinculacion-connect|Instalar y vincular el ordenador]]
- [[licencia-y-prueba-connect|Licencia y prueba gratuita]]
