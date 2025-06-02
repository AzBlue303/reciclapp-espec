# ADR-11: Reconocimiento de botellas plásticas
## Situación: 
Propuesto 
## Contexto:
El sistema debe permitir que los usuarios tomen fotos de botellas plásticas y sean reconocidas automáticamente para ganar puntos además de escanear un código QR para confirmar que están en el punto de reciclaje. Para ello se propone el uso de una IA especializada para el reconocimiento de las botellas, Existen APIs especializadas como Google Vision o Azure Computer Vision que pueden realizar este tipo de tareas con alto nivel de precisión.
## Decisión:
Se utilizará una API de visión artificial externa … para procesar las imágenes enviadas por los usuarios y detectar si se trata de una botella plástica.
## Consecuencias:
El tiempo de desarrollo será reducido al solo ser la implementación de la API, además entregará resultados con alto porcentaje de precisión pero debido a que es sobre IA probablemente tenga costos asociados al uso que se le dé o en caso de que la API dejé de estar disponible generaría problemas en producción.
## Cumplimiento:
Se establecerán pruebas de disponibilidad y tiempo de respuesta de la API, se mantendrá registro de errores relacionados a la API y evaluar el nivel de precisión antes de su integración con el sistema. 
## Notas: 
Autor:  Francisca Neira f.neira04@ufromail.cl <br />
Día de publicación:  01/06/2025 <br />
Última Actualización: 01/06/2025
