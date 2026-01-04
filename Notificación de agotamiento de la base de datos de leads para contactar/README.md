# 📉 Automatización de Alerta por Agotamiento de Base de Leads (n8n)

Este flujo en n8n monitorea de forma automática la cantidad de registros restantes en la base de datos de leads. Cuando detecta que quedan menos de 40 registros por procesar, envía una notificación al equipo a través de un chat corporativo de Gmail (API) para que preparen con antelación una nueva base de datos, evitando interrupciones en el flujo de trabajo.

## 🔧 Funcionalidades principales:

- ⏰ Ejecución periódica automática mediante Schedule Trigger.
- 📊 Lectura de la base de datos de leads alojada en Google Sheets.
- 📉 Cálculo de registros pendientes por procesar.
- 🔍 Verificación condicional: si hay menos de 40 empresas, se activa la alerta.
- 📨 Notificación automática al equipo vía Google Chat (API HTTP Request).
- 🔕 Prevención de notificaciones innecesarias cuando aún hay suficientes registros.

## 💡 Casos de uso:

Ideal para equipos que trabajan con listas de prospectos y desean mantener la continuidad operativa sin tiempos muertos. Esta automatización permite anticiparse al agotamiento de leads, asegurando que siempre haya una base lista para las siguientes campañas o tareas.
