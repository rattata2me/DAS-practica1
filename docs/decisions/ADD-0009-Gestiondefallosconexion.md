# Monitoreo de gestion fallos de conexion

* Status: proposed
* Date: 2022-11-22

Technical Story: RF-10

## Context and Problem Statement

Se requiere un sistema capaz de gestionar los fallos de conexion. El sistema de monitoreo tiene que ser capaz de gestionar los fallos de conexion.

## Considered Options

* ADD-0009.1 Desarrollo de un pequeño monitor de Dead Letter Queue de Apache Kaftka
* ADD-0009.1 Uilización de Prometheus integrado en el sistema de Kaftka
* ADD-0009.3 Uilización de Kaftka Connect

## Decision Outcome

Chosen option: "", because comes out best.

## Pros and Cons of the Options

### ADD-0009.1 Desarrollo de un pequeño monitor de Dead Letter Queue de Apache Kaftka
* Good, because Relativamente sencillo.
* Good, because Cumple con la especificación y puede hacer uso de frameworks de terceros.
* Bad, because Mayor complejidad en el desarrollo y problemas con reglas avanzadas.

### ADD-0009.2 Uilización de Prometheus integrado en el sistema de Kaftka

* Good, because Compatibilidad con cualquier solución.
* Bad, because Complejidad pues requiere una dependencia con utilización de kubernetes.
* Bad, because Problemas de sincronización con Kaftka y redundancia.

### ADD-0009.3 Uilización de Kaftka Connect
* Good, because Relativamente sencillo, aún más que un monitor de DLQ de terceros.
* Good, because Cumple con la especificación y permite trabajar con reglas futuras más avanzadas.
* Bad, because Excesivo para las reglas requeridas.
* Bad, because Mayor carga a Kaftka y problemas de complejidad arquitectonica.