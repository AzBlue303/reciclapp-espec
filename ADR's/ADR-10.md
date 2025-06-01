# ADR-10: Estructura de comunicacion Vista-API-Datos
## Situación: 
Propuesto 
## Contexto:
Dado que la aplicación implementará una API se requiere definir de qué manera se van a transmitir los datos desde esta.
## Decisión:
Se decidió implementar un patrón arquitectónico MVP (Model View Presenter) donde el presenter será la API, para definir la transferencia de datos pedidos desde la vista hacia la API.
## Consecuencias:
Implementar este patrón arquitectónico permitirá que las peticiones y los datos deban pasar por la API, esto dado que la API cumplirá el rol de Presenter y configurará los datos para que la View pueda verlos. Sin embargo, este modelo puede dificultar su testeo, dado que el Presenter gestiona tanto la entrada de la vista como la información recibida de la base de datos.
## Cumplimiento:
Se configurará la API para que cumpla el rol de Presenter, configurando tanto la petición de la Vista como la información recibida de la base de datos.
## Notas: 
Autor: Ignacio Pérez i.perez06@ufromail.cl <br />
Día de publicación: 01/06/2025 <br />
Última Actualización: 01/06/2025
