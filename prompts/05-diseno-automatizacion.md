# Prompt 05 — Diseño de una automatización empresarial

## 1. Objetivo

Utilizar Inteligencia Artificial para diseñar conceptualmente una automatización de registro de pedidos mediante herramientas No-Code, sin necesidad de programar.

Este ejercicio continúa el análisis realizado en el Prompt 04, pasando de identificar oportunidades de automatización a diseñar un proceso concreto.

## 2. Contexto del caso

Una pequeña empresa ficticia recibe aproximadamente 30 pedidos diarios por WhatsApp.

El equipo está compuesto por dos personas que registran manualmente los pedidos en Google Sheets.

Se busca reducir tareas repetitivas y errores de transcripción mediante una solución sencilla, económica y adecuada para principiantes.

El ejercicio consiste en diseñar la automatización, no implementarla.

## 3. Prompt original utilizado

Actuá como un consultor especializado en automatización de procesos empresariales mediante herramientas No-Code y Low-Code, con experiencia en Make, n8n y Google Sheets.

**CONTEXTO**

Una pequeña empresa comercial recibe aproximadamente 30 pedidos diarios por WhatsApp y tiene dos personas trabajando.

Actualmente, los pedidos se registran manualmente en Google Sheets, lo que consume tiempo y puede generar errores de transcripción.

En una evaluación anterior se identificó que automatizar el registro de pedidos sería una oportunidad de mejora.

La empresa todavía no utiliza herramientas de automatización y busca una solución económica, sencilla de mantener y adecuada para principiantes.

**OBJETIVO**

Diseñá una automatización que permita registrar pedidos previamente estructurados en Google Sheets, sin necesidad de transcribir manualmente cada dato.

No es necesario implementar la automatización. Necesito un diseño técnico y operativo comprensible para una persona sin experiencia en programación.

**REQUISITOS**

1. Proponé una forma sencilla de ingresar los pedidos estructurados, por ejemplo mediante Google Forms.
2. Compará brevemente Make y n8n, explicando cuál sería más conveniente para este caso y por qué.
3. Diseñá el flujo completo desde la recepción de un pedido hasta su registro en Google Sheets.
4. Identificá qué datos debe contener cada pedido: identificador único, fecha, producto, cantidad, precio, canal y estado.
5. Explicá cómo validar datos obligatorios, cantidades, precios y posibles pedidos duplicados.
6. Indicá qué debe suceder si un pedido está incompleto, contiene información incorrecta o falla la conexión con Google Sheets.
7. Definí qué tareas requieren intervención humana y cuáles pueden automatizarse mediante reglas.
8. Proponé dos indicadores medibles para evaluar el funcionamiento del proceso.

**FORMATO DE RESPUESTA**

Organizá la respuesta en las siguientes secciones:

- Comparación de herramientas.
- Herramienta recomendada y justificación.
- Flujo de automatización paso a paso.
- Estructura propuesta para Google Sheets.
- Manejo de errores y duplicados.
- Dos indicadores de evaluación.
- Prueba de funcionamiento con ejemplos.

**CASOS DE PRUEBA**

Pedido A:
- ID: PED-001
- Producto: Lente Aviador Negro
- Cantidad: 2
- Precio unitario: $15.000
- Canal: WhatsApp

Pedido B:
- ID: PED-002
- Producto: Lente Deportivo Azul
- Cantidad: no informada
- Precio unitario: $20.000
- Canal: WhatsApp

Pedido C:
- ID: PED-001
- Producto: Lente Aviador Negro
- Cantidad: 2
- Precio unitario: $15.000
- Canal: WhatsApp

El pedido C es un duplicado del pedido A.

Explicá qué debería suceder con cada pedido y por qué.

**RESTRICCIONES**

- No supongas que existe una integración directa con WhatsApp.
- No inventes precios ni capacidades de Make o n8n.
- Diferenciá las funciones verificadas de las que requieren una comprobación técnica.
- No permitas que pedidos incompletos se registren como confirmados.
- No permitas que un pedido duplicado genere dos registros válidos.
- No supongas que registrar un pedido significa que existe stock disponible.
- No incluyas datos personales reales de clientes.
- No afirmes que el sistema está implementado o funcionando: se trata de un diseño conceptual.
- Si una decisión técnica depende de información faltante, explicá qué debería verificarse antes de implementarla.

## 4. Primera ejecución y validación

**Modelo utilizado:** Google Gemini.

**Método:** ejecución del prompt y evaluación de seis criterios definidos previamente.

### Resultado inicial

Gemini recomendó utilizar Make para automatizar el registro de pedidos previamente estructurados mediante Google Forms y Google Sheets.

Propuso validar campos obligatorios, detectar identificadores duplicados y registrar pedidos que cumplieran las condiciones.

También identificó tareas de supervisión humana y dos indicadores de rendimiento.

### Evaluación

| Criterio | Resultado |
|---|---|
| Comparación de Make y n8n | Cumplido |
| Diseño del flujo y estructura de datos | Cumplido |
| Identificación de errores y duplicados | Cumplido |
| Manejo de fallas técnicas | Cumplido |
| Diferenciación entre automatización y supervisión humana | Cumplido |
| Indicadores y resolución correcta de todos los casos | Parcial |

**Resultado inicial: 5 de 6 criterios cumplidos.**

Se detectó que el modelo no distinguía suficientemente el registro de un pedido de su confirmación después de verificar el stock.

También se identificaron afirmaciones técnicas sobre reintentos automáticos y prevención de duplicados que requerían mayor precisión.

## 5. Segunda iteración

Se solicitó a Gemini que corrigiera tres aspectos:

1. Diferenciar los estados de recepción, validación de stock y confirmación.
2. Aclarar los requisitos y límites de los reintentos automáticos.
3. Revisar los riesgos de registros duplicados cuando existen operaciones simultáneas.

La segunda respuesta incorporó un flujo de estados más preciso, reconoció la necesidad de configurar mecanismos de recuperación y propuso medidas para reducir el riesgo de duplicados.

## 6. Resultados de los casos de prueba

| Pedido | Resultado esperado | Resultado de Gemini tras la corrección |
|---|---|---|
| PED-001 — A | Registrar como pendiente de stock | Cumplido |
| PED-002 — B | Derivar a revisión por falta de cantidad | Cumplido |
| PED-001 — C | Detectar duplicado y evitar segunda inserción válida | Cumplido conceptualmente |

**Resultado de la segunda evaluación: 6 de 6 criterios cubiertos entre ambas respuestas.**

## 7. Indicadores de rendimiento propuestos

**KPI 1 — Tiempo promedio de registro por pedido**

Permite comparar el tiempo administrativo utilizado para registrar pedidos antes y después de incorporar la automatización.

**KPI 2 — Tasa de errores de registro**

Permite medir discrepancias, registros incorrectos y duplicados en relación con el total de pedidos procesados.

Estos indicadores todavía no contienen resultados medidos, ya que la automatización no fue implementada.

## 8. Limitaciones técnicas

El ejercicio representa un diseño conceptual y no demuestra el funcionamiento de una integración real.

Antes de implementarlo sería necesario verificar:

- La configuración exacta de los conectores de Google Forms y Google Sheets.
- Los costos y límites de uso de Make.
- El almacenamiento y los reintentos de ejecuciones fallidas.
- Los mecanismos de procesamiento secuencial y prevención de duplicados.
- La validación de stock antes de confirmar pedidos.
- Los permisos de acceso y la protección de los datos.

La documentación oficial de Make distingue entre ciclos de ejecución, procesamiento de escenarios y mecanismos de reintento. Configurar un solo ciclo no garantiza por sí mismo que se eviten ejecuciones simultáneas.

Fuentes de consulta:

- https://help.make.com/scenario-settings
- https://help.make.com/automatic-retry-of-incomplete-executions
- https://help.make.com/retry-error-handler

## 9. Conclusiones y aprendizajes

La primera ejecución generó un diseño comprensible, pero presentó imprecisiones en aspectos relevantes para la operación empresarial.

Mediante una segunda iteración, fue posible mejorar la lógica de los estados de pedidos y reconocer limitaciones técnicas que necesitarían pruebas adicionales.

**Aprendizaje principal:** diseñar una automatización requiere contemplar no solamente el funcionamiento esperado, sino también los errores, los casos excepcionales, la integridad de los datos y la intervención humana.

El ejercicio permitió practicar la especificación de procesos, la definición de reglas y la validación de propuestas generadas mediante IA.

**Estado:** validación conceptual superada mediante dos iteraciones. Implementación técnica pendiente.
