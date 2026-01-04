# 🤖 Automatización: Seguimiento a Leads sin Respuesta

Este workflow en n8n realiza un follow-up automatizado a leads que no han respondido al primer correo con una propuesta de negocio. El flujo se ejecuta de forma programada y sigue los siguientes pasos:

1. **Trigger programado**: Inicia el flujo en una fecha/hora específica.
2. **Lectura de Google Sheets**: Se obtienen los leads desde una hoja de cálculo.
3. **Filtrado de leads sin respuesta**: Se identifican los que llevan más de 2 semanas sin contestar.
4. **Limitador de envíos**: Controla cuántos correos se enviarán en cada ejecución para no saturar el envío.
5. **Loop por cada lead**:
- Se preparan variables del mensaje.
- Se consulta el hilo del correo anterior con Gmail.
- Si el lead no ha respondido:
  - Se genera una plantilla de seguimiento.
  - Se responde al correo anterior con el nuevo mensaje.
  - Se actualiza el estado del lead en la hoja de cálculo.
- Si ya respondió, no se realiza ninguna acción.

## 💡 Casos de uso 
✅ Ideal para automatizar seguimientos comerciales y mantener una comunicación constante sin esfuerzo manual.
