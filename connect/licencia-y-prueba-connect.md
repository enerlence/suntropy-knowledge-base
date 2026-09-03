# Licencia, prueba gratuita y precio de Suntropy Connect

Suntropy Connect **no va incluido en los [[planes-de-suscripcion|planes de Suntropy]]**: es
una suscripción aparte, por persona, sin mínimos ni permanencia.

Todo esto se gestiona en la pantalla **`/pvsyst-plan`** de Suntropy, también accesible desde
**Configuración → Plan → Complementos**.

## Prueba gratuita

- **7 días**, sin tarjeta.
- Da acceso a todo: las 22 herramientas de PVsyst, las 7 de PV\*SOL y los 6 flujos
  preparados.
- Al acabar **no se convierte en nada**: si no se ha añadido una forma de pago, se cancela
  sola. Pasa a Individual sólo si la persona lo pide.
- **Es una por empresa, no una por usuario.** La licencia pertenece a la cuenta (al cliente),
  no a quien pulsa el botón: si un compañero ya la activó, la prueba de esa empresa está
  consumida y no se puede volver a empezar.

## Plan Individual

| Facturación | Precio |
|---|---|
| Anual | **18 €/mes** por usuario (216 €/año) |
| Mensual | **22,50 €/mes** por usuario |

Incluye los dos motores, los 6 flujos, actualizaciones y soporte, historial de trabajos, CSV
horario e informes.

## Servidor remoto

Para equipos que quieran PVsyst en modo servidor compartido, con un espacio por usuario y por
workspace, cola de trabajos y proyectos aislados por cliente. **Precio a consultar**: se
dimensiona y despliega con Suntropy.

## Dos licencias distintas, y no hay que confundirlas

La suscripción de Suntropy Connect **no incluye la licencia de PVsystCLI**. Son cosas
separadas:

- `run_simulation` y `run_batch` ejecutan PVsyst de verdad y consumen **cuota de la licencia
  de PVsystCLI del usuario**, que se contrata con PVsyst.
- Todo lo demás —leer resultados, gráficas, crear y editar proyectos— **no consume nada**.
- Ninguna consulta de PV\*SOL consume licencia, porque no ejecuta nada.

Un detalle útil: **un barrido en modo batch cuesta una sola llamada de licencia**, lleve las
simulaciones que lleve. Sale más a cuenta pedir un barrido que lanzar los casos uno a uno.

## Cuántos ordenadores a la vez

La licencia lleva un número de **plazas** (`seats`): son las personas que pueden estar
atendiendo **a la vez**, una por usuario.

- Un mismo usuario en dos ordenadores: el segundo **desplaza** al primero. No es un error, es
  el diseño: una persona, una plaza.
- Otro usuario cuando no quedan plazas: entra y **desaloja al menos activo**, medido por la
  última petición real, no por estar simplemente encendido.
- Al desplazado no se le avisa: se entera en su siguiente latido. Vuelve a conectar y ya
  está.

Vincular un ordenador **no ocupa plaza**; sólo la ocupa estar conectado.

## Documentos relacionados

- [[que-es-suntropy-connect|Qué es Suntropy Connect]]
- [[gestion-de-equipos-connect|Ver y desconectar equipos]]
- [[planes-de-suscripcion|Planes de Suntropy]]
- [[suscripcion-y-pagos|Suscripción y pagos]]
