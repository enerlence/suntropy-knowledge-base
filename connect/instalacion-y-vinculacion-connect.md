# Instalar Suntropy Connect y vincular el ordenador

Son tres pasos y se hacen una sola vez. Todo ocurre en el ordenador que ya tiene PVsyst o
PV\*SOL instalado: no hay nada que instalar en ningún servidor.

## Paso 1 — Descargar e instalar

Descarga en **https://connect.suntropy.ai/download** (o el botón "Descargar para Windows" de
https://connect.suntropy.ai). El instalador es `PVsystConnect-Setup.exe`, unos 190 MB, y
**no pide permisos de administrador**.

Al instalarse detecta solo la instalación de PVsyst y su versión, y busca las carpetas de
proyectos de PV\*SOL. Si alguna carpeta no aparece, se puede añadir a mano desde el programa.

## Paso 2 — Aprobar el código

Al abrirlo, el programa muestra un **código de emparejamiento** de ocho caracteres con un
guion en medio, del tipo `WXYZ-1234`, y abre el navegador en la pantalla de aprobación.

Esa pantalla es **`/link-device`** en Suntropy. Ahí se ve qué ordenador pide conectarse y de
qué cuenta es, y se aprueba con el botón **Aprobar**.

Tres cosas que conviene saber, porque son las que más se preguntan:

- **El código caduca a los 10 minutos.** Si se pasa el rato, no hay nada que arreglar: se
  vuelve al programa, que muestra uno nuevo.
- **Si no hay sesión iniciada**, Suntropy pide entrar (o crear cuenta y validar el correo) y
  devuelve después a la misma pantalla, con el código intacto.
- **El código se puede teclear a mano** en `/link-device` si el navegador se cerró o se abrió
  en otro equipo. La pantalla tiene un campo para escribirlo.

Una vez aprobado, el ordenador queda vinculado **90 días**, y se renueva solo mientras se
use.

## Paso 3 — Conectar el asistente

Queda dar de alta la dirección en Claude o en ChatGPT. Va en
[[conectar-claude-y-chatgpt|su propio documento]].

## No tengo ningún código

Es la situación de quien se ha creado la cuenta desde la web de Connect y todavía no ha
instalado nada. **El código lo da el programa**: hasta instalarlo no hay ninguno que
escribir. La propia pantalla de `/link-device` ofrece la descarga justo debajo del campo del
código.

El orden correcto es: instalar en el ordenador que tiene PVsyst o PV\*SOL → abrir el programa
→ aprobar el código que muestre.

## Documentos relacionados

- [[que-es-suntropy-connect|Qué es Suntropy Connect]]
- [[licencia-y-prueba-connect|Licencia y prueba gratuita]]
- [[problemas-frecuentes-connect|Problemas frecuentes]]
