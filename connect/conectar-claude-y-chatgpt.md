# Conectar Claude o ChatGPT a Suntropy Connect

Con el ordenador ya vinculado ([[instalacion-y-vinculacion-connect|paso previo]]), queda dar
de alta una dirección en el asistente. Hay **una dirección por motor**, y se pueden tener las
dos a la vez.

| Motor | Dirección |
|---|---|
| PVsyst | `https://pvsyst-connect-gateway.suntropy.ai/pvsyst/mcp` |
| PV\*SOL | `https://pvsyst-connect-gateway.suntropy.ai/pvsol/mcp` |

## En Claude

Es el mismo sitio en Claude Code, en la app de escritorio y en claude.ai.

1. **Ajustes → Conectores**.
2. **Añadir conector personalizado**: un nombre (`PVsyst` o `PV*SOL`) y la dirección de
   arriba. Nada más.
3. Se enciende desde el menú **«+»** de la conversación, junto a las demás fuentes. Se activa
   por conversación.

## En ChatGPT

Es el mismo sitio en chatgpt.com y en la app de escritorio.

1. **Plugins → Conectar plugins**.
2. **Nuevo plugin**: nombre, la dirección de arriba y autenticación **OAuth**.
3. Se activa desde el menú **Plugins** de la conversación.

## La primera vez pedirá entrar

Al usarlo por primera vez, el asistente abre el navegador para que la persona se identifique
con su cuenta de Suntropy. Es la misma cuenta con la que se aprobó el ordenador; si la
licencia no está en vigor, ahí es donde se nota.

## Documentos relacionados

- [[que-es-suntropy-connect|Qué es Suntropy Connect]]
- [[problemas-frecuentes-connect|Problemas frecuentes]]
