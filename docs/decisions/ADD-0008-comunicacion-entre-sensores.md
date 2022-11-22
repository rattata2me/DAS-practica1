# Envío de información entre sensores de la familia IoT

* Status: proposed
* Date: 2022-11-22

Technical Story: RF-11

## Context and Problem Statement

Se quiere enviar información entre los tres sensores IoT: que el primero envíe información al segundo y el segundo al tercero. Además queremos organizar los sensores en familias.

## Considered Options

* ADD-0008.1 Utilizar un sistema por capas en los sensores IoT de cada familia.

## Decision Outcome

Chosen option: "Utilizar un sistema por capas en los sensores IoT de cada familia", because comes out best.

## Pros and Cons of the Options

### ADD-0008.1 

* Good, because Existe separación de responsabilidades.
* Good, because Estilo arquitectónico conocido y, por tanto, fácil de desarrollar (reutilización).
* Bad, because Menos eficiente.
* Bad, because Posible redundancia entre capas.
* Bad, because A veces requiere una cascada de cambios en las capas.

