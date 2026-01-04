# 📬 Automatización de Notificación de Correos No Respondidos (n8n)

Este flujo en n8n detecta automáticamente correos electrónicos importantes que no han sido respondidos en más de 2 días y notifica al equipo interno a través de un chat corporativo conectado mediante la API de Gmail Chat, asegurando que ningún mensaje relevante quede sin atención.

## 🔧 Funcionalidades principales:

- ✅ Ejecución programada automática mediante nodo de tipo Schedule Trigger.
- 📥 Búsqueda de correos sin responder utilizando la API de Gmail.
- ⏳ Filtrado por antigüedad para detectar correos sin contestar desde hace más de 2 días.
- 📂 Consulta cruzada con registros de notificaciones previas para evitar notificaciones duplicadas.
- 📨 Notificación automática al equipo vía mensaje en un canal de Google Chat (API HTTP Request).
- 📬 Filtrado de correos válidos para garantizar que solo se notifiquen mensajes relevantes.
- ✏️ Organización y personalización del contenido del mensaje enviado al equipo.
- 🧾 Registro del correo notificado en hoja de cálculo para trazabilidad.
- ⏱️ Espera configurada para control de ejecución en bucles.

## 💡 Casos de uso:

Ideal para equipos comerciales, de atención al cliente o soporte técnico que reciben múltiples correos y quieren garantizar una atención rápida a leads, clientes o contactos importantes. Esta automatización reduce el riesgo de perder oportunidades por falta de respuesta o seguimiento.
