# Base de datos de sensores

* Status: accepted
* Date: 2022-11-15

Technical Story: RF-1, RF-5

## Context and Problem Statement

Se requiere un sistema capaz de guardar los datos en una base de datos con el fin de poder ser utilizados mas a delante

## Considered Options

* ADD-0005.1 Base de datos relacional
* ADD-0005.2 Base de datos no relacional basada en llaves

## Decision Outcome

Chosen option: "Utilización de base de datos relacional", because comes out best.

## Pros and Cons of the Options

### ADD-0005.1 Base de datos relacional

* Good, comunmente usadas en cualquier campo.
* Bad, because ligeramente más lentas y pesadas para tan solo recoger datos de sensores y ordenes de trabajo.

### ADD-0005.2 Base de datos no relacional basada en llaves

* Good, because rápida y segura.
* Bad, because No permite consultas complicadas.

