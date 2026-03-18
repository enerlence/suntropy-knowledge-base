# Integraciones

Suntropy ofrece diversas integraciones con servicios externos. Se configuran en **Configuracion > Integraciones**.

## Integraciones disponibles

### Datadis
Importa [[curvas-de-consumo|curvas de consumo]] reales del cliente directamente desde la base de datos de distribuidoras electricas. Requiere tener usuario y contrasena de Datadis configurados en la plataforma.

### SMTP personalizado
Configura tu proveedor de correo para que los emails enviados al cliente (estudios, presupuestos) lleven el **dominio de tu empresa** en lugar del de Suntropy. Util para dar imagen de marca profesional.

### CRM (Odoo, Zoho, HubSpot, etc.)
Integra tu CRM a traves de **webhooks** o **Akiki** para sincronizar datos de clientes y estudios automaticamente. Permite:
- Enviar datos de estudios al CRM
- Recibir datos de clientes desde el CRM
- Automatizar flujos de trabajo

### Firma digital
Envia presupuestos para ser firmados digitalmente por el cliente. Los documentos originales y firmados quedan almacenados en **Herramientas > [[gestion-documentos|Documentos]] > Firmas digitales**.

### Pontio (financiacion)
Integra con Pontio para ofrecer opciones de financiacion directamente desde el balance economico del estudio de [[autoconsumo-individual]].

### Calculadora Solar (Solar Form)
Si tienes contratada la calculadora solar embebible en tu web, configurala desde el apartado **"Mas"** en el menu principal. Es un micrositio whitelabel conectado con el backend de Suntropy.

## SMTP y Calculadora Solar

Cuando un cliente usa la calculadora solar y deja sus datos, se genera un pre-estudio que se envia a su correo. Si el SMTP esta configurado, ese correo llegara con el dominio de la empresa.

## Automatizaciones

Las automatizaciones para integrar CRM se configuran en **Configuracion > Automatizaciones**. Se puede hacer a traves de:
- **Webhooks**: Envio directo de datos entre sistemas
- **Akiki**: Plataforma de integracion para conectar multiples servicios

---

> **Para ampliar informacion, busca en los PDFs adjuntos:**
> - `Configuracion (2).pdf` - Video "Conoce todas las configuraciones de tu perfil de usuario" con detalle de como configurar Datadis (usuario/contrasena), SMTP personalizado (datos del proveedor web), estudios predeterminados (precios, perdidas, impuestos, ratio, margen, excedentes, distancia paneles, parametros optimizacion, panel/kit por defecto, subvenciones), tema (logo y colores), notificaciones (campanita y/o email), y automatizaciones (webhooks y Akiki)
