# ADR-8: Importancia de la robustez en el sistema
## Situación: 
Propuesto
## Contexto: 
El sistema trabaja con sensores, por lo que estos pueden fallar o dejar de funcionar.
## Decisión: 
Por lo que se decide construir un sistema robusto para que este pueda seguir funcionando independientemente de los sensores.
## Consecuencias:
Al ser un sistema robusto se asegura su funcionamiento incluso si empiezan a fallar los sensores. Sin embargo, al implementar esto, se requerirá aumentar la complejidad del código, añadiendo funciones extra que eviten esta caída.
## Cumplimiento:
La implementación de estas funcionalidades se realizará durante la construcción de las funciones que pueden caer junto con el sensor fallido.
## Notas:
Autor: Ignacio Pérez i.perez06@ufromail.cl <br />
Día de publicación: 01/06/2025 <br />
Ultima Actualización: 01/06/2025
