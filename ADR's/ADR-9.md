# ADR-9: Estructura de comunicación Vista-Datos
## Situación: 
Propuesto 
## Contexto: 
Se requiere definir una manera de comunicación entre las vistas y los datos almacenados.
## Decisión:
Se decidió utilizar un estilo arquitectónico implementando una Capa de API, ingresando a este tercero para unir la conexión entre las vistas y los datos.
## Consecuencias:
Implementar una API permitirá mantener la comunicación entre vistas-datos, centrando que solo se acceda a los datos necesarios y/o permitidos. Sin embargo, utilizar una API puede generar problemas de seguridad, ya que los datos se moverán de un punto a otro.
## Cumplimiento:
Se implementarán métodos de seguridad para prevenir que se inyecten datos no autorizados y/o ingresados por administradores oficiales.
## Notas: 
Autor: Ignacio Pérez i.perez06@ufromail.cl <br /> 
Día de publicación: 01/06/2025 <br />
Última Actualización: 01/06/2025
