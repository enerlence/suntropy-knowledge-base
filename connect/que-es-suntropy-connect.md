# Qué es Suntropy Connect

Suntropy Connect es un programa de escritorio para Windows que conecta el **PVsyst** o el
**PV\*SOL** que ya están instalados en el ordenador del usuario con un asistente de IA
(Claude o ChatGPT). A partir de ahí se le puede pedir en lenguaje natural que simule, que
compare variantes o que resuma resultados, y el asistente trabaja contra los proyectos
reales del disco.

Es un producto de Suntropy, no una integración de terceros. Vive en
https://connect.suntropy.ai y se contrata aparte del plan de Suntropy: ver
[[licencia-y-prueba-connect|licencia y prueba]].

## La idea en una frase

**La licencia, el ordenador y los proyectos se quedan donde están.** Connect no sube nada:
abre una conexión saliente desde el equipo del usuario —sin abrir puertos ni tocar el
router— y por ahí atiende lo que el asistente le pide. Se revoca desde la web cuando se
quiera (ver [[gestion-de-equipos-connect|gestión de equipos]]).

## Dos motores, y no hacen lo mismo

Esta es la distinción que más confusión genera, y conviene decirla antes que ninguna otra:

| | **PVsyst** | **PV\*SOL** |
|---|---|---|
| Qué hace | Simula, crea y edita proyectos | **Sólo lee** proyectos ya simulados |
| Herramientas | 22 | 7 |
| Resolución | Horaria, con CSV descargable | **Mensual**, 12 valores por magnitud |
| Variantes | Sí (VC0, VC1…) | No: un `.pvprj` es un proyecto y una configuración |
| Consume licencia | Sólo `run_simulation` y `run_batch` | Nunca |

Que PV\*SOL sólo lea **no es una limitación temporal ni una funcionalidad pendiente**: PV\*SOL
no tiene línea de comandos ni API de cálculo, así que no hay forma de ejecutarlo sin su
interfaz gráfica. Lo que sí hace PV\*SOL, y PVsyst no, es guardar los resultados **dentro**
del propio proyecto: por eso un proyecto ya simulado devuelve producción, autoconsumo,
excedentes, cobertura solar, PR y la cascada completa de pérdidas sin ejecutar nada.

Si un proyecto de PV\*SOL nunca se ha simulado, su fichero no lleva resultados y de ése no
hay número que dar.

## Qué se puede pedir

Sobre PVsyst, además de leer proyectos y resultados: lanzar una simulación, barrer hasta 21
parámetros de sistema en modo batch, crear proyectos nuevos a partir de una plantilla,
editar variantes y descargar el informe PDF de PVsyst y el CSV horario.

Vienen además **6 flujos preparados**: optimizar orientación, auditar una variante, comparar
dos variantes, generar un informe, cartera multi-sitio e informe visual.

## Requisitos

- Windows 10 u 11.
- Para PVsyst: **PVsyst 8.x** instalado y con licencia activa.
- Para PV\*SOL: PV\*SOL premium con proyectos `.pvprj` ya simulados.
- Cuenta de Suntropy (la misma de la plataforma).
- Claude Code, la app de escritorio de Claude o claude.ai; o ChatGPT web o de escritorio.

## Documentos relacionados

- [[instalacion-y-vinculacion-connect|Instalar y vincular el ordenador]]
- [[conectar-claude-y-chatgpt|Conectar Claude o ChatGPT]]
- [[licencia-y-prueba-connect|Licencia, prueba gratuita y precio]]
- [[gestion-de-equipos-connect|Ver y desconectar equipos]]
- [[problemas-frecuentes-connect|Problemas frecuentes]]
