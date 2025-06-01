# ADR-5:  Obtención de mapas
## Situación: 
Propuesto 
## Contexto:
Se debe utilizar un mapa para visualizar la ubicación del usuario y de los contenedores dentro de la aplicación y página web.
## Decisión:
Se utilizará la API OpenStreetMap usando la biblioteca Leaflet, de la cual se obtiene un mapa para poder mostrar los contenedores a los usuarios. Esta API en particular permite ubicar varios puntos en el mapa, lo que nos permite mostrar varios contenedores al mismo tiempo y es abierta al público facilitando su implementación.
## Consecuencias:
Utilizar una API para obtener el mapa nos garantiza que sea confiable para el usuario pero la utilización de Leaflet, al ser una api pública corre el riesgo de no tener soporte a futuro.
## Cumplimiento:
Se harán pruebas para comprobar que se obtienen correctamente los mapas y que estos estén actualizados.
## Notas: 
Autor: Francisca Neira f.neira04@ufromail.cl <br />
Día de publicación: 28/05/2025 <br />
Última Actualización: 28/05/2025
