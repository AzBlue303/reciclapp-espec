# ADR-3: Base de datos del sistema
## Situación: 
Propuesto. 
## Contexto: 
Al tener que almacenar 2 elementos completamente distintos en base de datos, los cuales son credenciales de administradores y datos enviados por el sensor, y es recomendable evitar el uso de dos bases de datos distintas, hay que utilizar una que permita el almacenamiento de ambos tipos de datos.
## Decisión: 
Se decidió utilizar PostgreSQL con PostGIS para las coordenadas de los sensores y JSON Types para almacenar los datos de cada sensor.
## Consecuencias: 
Utilizar PostgreSQL hace más seguro el almacenamiento de las credenciales de los administradores, lo que puede evitar hackeos o robos de estas, también evita la creación de funcionalidades para el filtrado de datos cercanos al usuario ya que vienen integrados con PostGIS. Sin embargo se hace necesario optimizar las consultas sobre los datos enviados de los sensores, dado que a medida que estos vayan creciendo se hará más complejo obtener información.
## Cumplimiento: 
Creando índices con índices GIN de PostgresSQL permite que la búsqueda de datos sea más óptima, y al utilizar PostGIS (Geographic Information Systems) se podrá filtrar los sensores por la ubicación geográfica del usuario.
## Notas: 
Autor: Ignacio Pérez i.perez06@ufromail.cl<br />
Día de publicación: 28/05/2025 <br />
Última Actualización: 28/05/2025
