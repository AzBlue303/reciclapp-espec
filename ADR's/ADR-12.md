# ADR-12: Formato de datos para interoperabilidad
## Situación: 
Propuesto 
## Contexto:
El sistema se compone de múltiples componentes tecnológicos como sensores IoT, aplicación móvil, página web administrativa, APIs de terceros como mapas, entre otros. Debido a esto se debe definir un formato de intercambio de datos común que garantice la interoperabilidad y facilite el mantenimiento.
## Decisión:
Se utilizará JSON como formato estándar para el intercambio de datos entre todos los componentes del sistema. Este formato será usado en todas las comunicaciones internas y externas del sistema.
## Consecuencias:
Permite una integración sencilla entre los componentes externos e internos del sistema, JSON es legible al ojo humano lo que permite que sea sencillo de entender en depuraciones o testing pero los datos podrían dañarse o perderse en el cambio de formato, podría retardar la comunicación entre componentes
## Cumplimiento:
Se validarán los datos antes y después de ser formateados para asegurar su integridad, se realizarán pruebas para garantizar un rendimiento óptimo, se documentará la estructura que seguirán los datos para evitar errores. Una vez aplicado se harán de integración para garantizar la interoperabilidad del sistema.
## Notas: 
Autor:  Francisca Neira f.neira04@ufromail.cl <br />
Día de publicación:  01/06/2025 <br />
Última Actualización: 01/06/2025