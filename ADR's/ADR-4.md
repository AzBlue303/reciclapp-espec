# ADR-4: Método de acceso a los datos de los sensores
## Situación: 
Propuesto 
## Contexto:
Se necesita una forma de comunicación entre los sensores y la base de datos para recibir y procesar los datos enviados.
## Decisión:
Se decide utilizar una API que se encargue de tres pasos esenciales, recibir los datos, pasarlos al formato adecuado para la base de datos y almacenarlos en ella.
## Consecuencias:
Utilizar una api nos garantiza manejar los datos antes de ser registrados en la base de datos.Sin embargo podría afectar el rendimiento de la aplicación retardando el tiempo de actualización.
## Cumplimiento:
Se realizarán pruebas para comprobar que el manejo de los datos es el correcto y el rendimiento es el adecuado para la aplicación.
## Notas: 
Autor:  Francisca Neira f.neira04@ufromail.cl <br />
Día de publicación:  28/05/2025 <br />
Última Actualización: 28/05/2025
