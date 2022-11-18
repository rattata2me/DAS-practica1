# IA Predictora

* Status: accepted
* Date: 2022-11-12

Technical Story: RF-7

## Context and Problem Statement

Se requiere gestionar y predecir los fallos de líneas de trabajo para poder enmendarlos correctamente.

## Considered Options

* ADD-0004.1 Utilización de redes neuronales y agentes QL para la predicción de fallos y reasignación de recursos.
* ADD-0004.2 Utilización de algoritmo con agente inteligente basado en Monte Carlo.
* ADD-0004.3 Utilización de Redes de Petri.

## Decision Outcome

Chosen option: "Utilización de redes neuronales y agentes QL para la predicción de fallos y reasignación de recursos", because comes out best.

## Pros and Cons of the Options

### ADD-0004.1 Utilización de redes neuronales y agentes QL para la predicción de fallos y reasignación de recursos.

* Good, because Resultados de alta precisión.
* Good, because Poca dependencia entre componentes.
* Bad, because Necesidad de mayor preprocesamiento de datos.
* Bad, because Alto tiempo de aprendizaje.

### ADD-0004.2 Utilización de algoritmo con agente inteligente basado en Monte Carlo.

* Good, because Directo y flexible.
* Good, because Al ser una simulación, no interfiere en resultados reales.
* Good, because Plantea una gran cantidad de escenarios en muy poco tiempo.
* Bad, because No proporciona una decisión concreta, solo resuelve el comportamiento. 
* Bad, because Cada simulación arroja datos diferentes, ya que son valores aleatorios.

### ADD-0004.3 Utilización de Redes de Petri.

* Good, because Buena visualización de las dependencias entre elementos del sistema
* Good because Análisis de comportamiento sin necesidad de simulación o ejecutar pruebas
* Bad, because Complejidad.
* Bad, because No es ambivalente.
* Bad, because Consume mucho tiempo y espacio en problemas complejos.

