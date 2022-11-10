# Sistema de mensajería

* Status: accepted
* Date: 2022-11-07

Technical Story: RF-9

## Context and Problem Statement

Se requiere de un sistema capaz de gestionar las subscripciones de los operarios. El sistema debe de ser capaz de permitir a los operarios suscribirse a eventos y notificaciones. ¿Qué alternativas cumplen con un patrón fiable para gestionar los mensajes?¿Qué sistema es capaz de gestionar los mensajes?

## Considered Options

* ADD-0002.1 Utilización de un sistema de mensajería de tipo publicar-suscribir. MQTT, STOMP, AMQP
* ADD-0002.2 Utilización de Apache Kaftka con aplicacion propietaria
* ADD-0002.3 Utilización de un servicio de notificación como AWS SNS, Google GCM o WNS

## Decision Outcome

Chosen option: "Utilización de Apache Kaftka"

## Pros and Cons of the Options

### ADD-0002.1 Utilización de un sistema de mensajería de tipo publicar-suscribir. MQTT, STOMP, AMQP

* Good, because Estándar en industria
* Good, because Jerarquía de sistemas
* Good, because Seguridad por ofuscación
* Bad, because Complejidad
* Bad, because Falta de abstracción

### ADD-0002.2 Utilización de Apache Kaftka

* Good, because Sencillez con plataformas estándar
* Good, because Buena abstracción
* Bad, because Más dependencias
* Bad, because Mayor flujo y complejidades con las jerarquías

### ADD-0002.3 Utilización de un servicio de notificación como AWS SNS, Google GCM o WNS

* Good, because Altamente sencillo
* Good, because Elástico y con alta disponibilidad
* Bad, because Problemas con la seguridad puesto que los mensajes pasarían a gestionarse de manera no interna.
* Bad, because Dependencia de más sistemas propietarios.
* Bad, because En función de la solución escogida, precio más alto a largo plazo.
* Bad, because Dependiente de conexiones a internet
