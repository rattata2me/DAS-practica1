# ADD-0001 Necesidad de sistema de eventos distribuido.

* Status: accepted
* Date: 2022-11-02

Technical Story: RF-12, RF-8

## Context and Problem Statement

Se requiere un sistema capaz de gestionar los eventos de una factoria inteligente en la que se registren datos y se notifiquen a los operarios. ¿Cómo gestionar el intercambio de información entre los distintos sensores y empleados, es decir de forma distribuida?

## Considered Options

* ADD-0001.1 - Sistema con control distribuido y módulo central
* ADD-0001.2 - Sistema basado en interacción por eventos.

## Decision Outcome

Chosen option: "Sistema basado en interacción por eventos.", because Se adecua perfectamente al problema descrito.

### Positive Consequences

* Mejor decisión a largo plazo
* Sencillez con microservicios

### Negative Consequences

* Dificultad para tareas de la fábrica asíncronas

## Pros and Cons of the Options

### ADD-0001.1 - Sistema con control distribuido y módulo central

* Good, because Estándar en industria
* Good, because Jerarquía de sistemas
* Good, because Seguridad por ofuscación
* Bad, because Complejidad
* Bad, because Falta de abstracción

### ADD-0001.2 - Sistema basado en interacción por eventos.

* Good, because Sencillez con plataformas estándar
* Good, because Buena abstracción
* Bad, because Más dependencias
* Bad, because Mayor flujo y complejidades con las jerarquías
