# Asignar órdenes de trabajo

* Status: proposed
* Date: 2022-11-22

Technical Story: RF-3, RF-4

## Context and Problem Statement

Necesitamos un módulo de órdenes de trabajo capaz de asignar órdenes a operarios y máquinas. 
Se requiere una interfaz sencilla que responda a los problemas de: crear, destruir y visualizar órdenes de trabajo por operario o máquina.
Por lo tanto, necesitamos una CMMS.

## Considered Options

* ADD-0007.1 Utilizar un SaaS como módulo externo
* ADD-0007.2 Diseñar un módulo CMMS
* ADD-0007.3 Utilizar el software ERPNext

## Decision Outcome

Chosen option: "", because comes out best.

## Pros and Cons of the Options

### ADD-0007.1 Utilizar un SaaS como módulo externo

* Good, because Sencillo de implementar, ya que es una solución preparada instantáneamente (menor coste de tiempo).
* Good, because Fácil de gestionar a largo plazo.
* Good, because Muy completa, no solo cubre el requisito si no que añade funcionalidades extras.
* Bad, because Mayor dependencia al ser un módulo externo.
* Bad, because Mayor coste económico a largo plazo.
* Bad, because Mayores problemas de seguridad.

### ADD-0007.2 Diseñar un módulo CMMS

*Good, because Opción que más se ajusta al problema propuesto.
*Good, because Opción que ofrece más control de seguridad y compatibilidad propietaria a largo plazo.
* Bad, because Coste elevado por la necesidad de desarrollo y mantenimiento constante.
* Bad, because Software mucho mas limitado que el resto de las opciones.
* Bad, because Solución con dificultades para ser escalable.

### ADD-0007.3 Utilizar el software ERPNext

* Good, because Relativamente sencilla de preparar aunque requiera de preparaciones y modificaciones en la instalación
* Good, because Muy completa, no solo cubre el requisito si no que añade funcionalidades extras.
* Good, because La más económica a largo plazo sin comprometer eficacia.
* Bad, because Requiere mantenimiento y actualizaciones de seguridad.