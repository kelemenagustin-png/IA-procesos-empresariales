# Prompt 03 — Comparación de herramientas de gestión de proyectos

## 1. Objetivo

Utilizar Inteligencia Artificial para comparar herramientas de gestión de proyectos y obtener una recomendación fundamentada según las características y limitaciones de un equipo pequeño.

El ejercicio fue desarrollado durante la clase 4 de Prompt Engineering de ITeducation.

## 2. Contexto del caso

Se plantea un equipo de trabajo compuesto por dos personas que todavía no utiliza una metodología formal de gestión de tareas y no tiene un presupuesto fijo definido.

El objetivo es evaluar qué herramienta sería más conveniente para comenzar a organizar el trabajo.

Las alternativas seleccionadas son:

- Trello.
- Asana.
- Jira.

## 3. Prompt original

Actua como una consultora en productividad para recomendarme una app de gestion de proyectos entre: Trello, Asana y Jira. Considerando las carectiristicas principales de cada herramienta, sus costos en sus servicios y la facibilidad de uso al comienzo para implementar en un equipo que se compone de 2 personas, sin presupuesto fijo, sin modalidades implementadas. Cual recomiendas y el por que de tu razonamiento?

## 4. Componentes del prompt

**Rol:** consultora en productividad.

**Tarea:** comparar tres aplicaciones de gestión de proyectos.

**Contexto:** equipo de dos personas sin metodología de gestión implementada.

**Criterios de comparación:** características principales, costos y facilidad de uso.

**Resultado esperado:** una recomendación justificada.

## 5. Validación del prompt

**Modelos utilizados:** ChatGPT y Google Gemini.

**Método:** ejecución del mismo prompt en dos modelos de lenguaje y comparación de las recomendaciones obtenidas.

### Resultados

| Criterio | ChatGPT | Gemini |
|---|---|---|
| Herramienta recomendada | Trello | Trello |
| Argumento principal | Simplicidad de implementación | Facilidad de aprendizaje y adopción |
| Tamaño del equipo | Considerado | Considerado |
| Costos | Se consideraron planes gratuitos | Se consideraron planes gratuitos |
| Facilidad de uso | Prioridad alta | Prioridad alta |
| Justificación | Recomendación contextualizada | Comparación y argumentación detallada |

### Verificación de la información

Se contrastaron los planes gratuitos con las páginas oficiales de cada herramienta:

- Trello: hasta 10 colaboradores y 10 tableros por espacio de trabajo.
- Asana: hasta 2 usuarios y proyectos ilimitados.
- Jira: hasta 10 usuarios en el plan gratuito.

Fuentes consultadas:

- https://trello.com/es/pricing
- https://asana.com/es/pricing
- https://www.atlassian.com/software/jira/pricing

Se identificó una afirmación incorrecta en la respuesta de Gemini: indicó que Trello permite tableros ilimitados en su plan gratuito, cuando el límite oficial es de 10 tableros por espacio de trabajo.

También afirmó que cualquier persona puede aprender a utilizar Trello en menos de cinco minutos, sin aportar evidencia que permita garantizar ese tiempo de aprendizaje.

### Criterios de evaluación

| Criterio | Resultado |
|---|---|
| Comparar Trello, Asana y Jira | Cumplido |
| Considerar los planes gratuitos | Cumplido |
| Evaluar la facilidad de uso | Cumplido |
| Considerar un equipo de dos personas | Cumplido |
| Proporcionar una recomendación justificada | Cumplido |
| Verificar la exactitud de toda la información | Parcial: se detectaron afirmaciones incorrectas o no fundamentadas |

### Conclusión de la validación

Ambos modelos recomendaron Trello, utilizando argumentos similares relacionados con su simplicidad y facilidad de implementación.

La verificación posterior mostró que una conclusión razonable puede estar acompañada de información incorrecta.

**Aprendizaje principal:** la coincidencia entre modelos no garantiza la exactitud de sus respuestas. Es necesario contrastar la información con fuentes confiables.

**Estado:** prueba comparativa realizada y verificación documental parcial completada.
