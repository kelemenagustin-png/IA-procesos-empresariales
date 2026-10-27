# Prompt 04 — Identificación de oportunidades de automatización

## 1. Objetivo

Explorar cómo la Inteligencia Artificial puede ayudar a identificar tareas repetitivas y oportunidades de automatización en pequeñas empresas.

El ejercicio busca diferenciar los procesos que pueden automatizarse mediante reglas de aquellos que podrían beneficiarse de modelos de IA.

## 2. Contexto del caso

Se plantea una pequeña empresa ficticia que recibe aproximadamente 30 pedidos diarios por WhatsApp.

Un equipo de dos personas administra manualmente los mensajes, la identificación de productos, la verificación de precios y stock, el registro de pedidos y las confirmaciones a los clientes.

Actualmente utiliza WhatsApp y Google Sheets, sin automatizaciones implementadas.

## 3. Prompt utilizado

### Prompt original completo

Actuá como un consultor especializado en optimización de procesos empresariales y automatización mediante Inteligencia Artificial.

**Contexto:**

Una pequeña empresa comercial recibe aproximadamente 30 pedidos diarios por WhatsApp.

Actualmente, una persona se encarga manualmente de:

1. Leer los mensajes de los clientes.
2. Identificar qué productos solicita cada cliente.
3. Verificar precios y disponibilidad.
4. Registrar los pedidos en Google Sheets.
5. Responder a los clientes con una confirmación.
6. Informar al responsable del negocio cuando falta mercadería.

La empresa tiene dos personas trabajando, utiliza WhatsApp y Google Sheets y no cuenta con automatizaciones implementadas.

**Objetivo:**

Analizá este proceso e identificá las oportunidades de automatización que podrían reducir tareas repetitivas, disminuir errores y mejorar la organización del trabajo.

**Instrucciones:**

1. Identificá qué tareas podrían automatizarse completamente, cuáles parcialmente y cuáles requieren supervisión humana.
2. Explicá por qué clasificaste cada tarea de esa manera.
3. Priorizá las tres oportunidades de automatización más convenientes para comenzar.
4. Indicá qué herramientas podrían utilizarse, considerando alternativas gratuitas o de bajo costo.
5. Diferenciá las automatizaciones basadas en reglas de aquellas que podrían necesitar IA.
6. Proponé dos indicadores para medir si la implementación produce mejoras.

**Formato de respuesta:**

Presentá una tabla con las columnas:

- Tarea.
- Tipo de automatización.
- Herramienta sugerida.
- Beneficio esperado.
- Riesgos o limitaciones.
- Prioridad.

Finalizá con una recomendación de los primeros tres pasos que debería realizar la empresa.

**Restricciones:**

- No asumas que todas las tareas necesitan Inteligencia Artificial.
- No inventes precios, capacidades ni integraciones de las herramientas sugeridas.
- No supongas que se puede acceder automáticamente a los mensajes de WhatsApp sin verificar los requisitos técnicos y permisos correspondientes.
- No recomiendes automatizar confirmaciones de pedidos sin verificar previamente precios y disponibilidad.
- Considerá la privacidad de los datos de los clientes.
- No garantices ahorros de tiempo ni mejoras sin contar con mediciones iniciales.
- Priorizá soluciones sencillas y realistas para un equipo de dos personas.

## 4. Validación del prompt

**Modelo utilizado:** Google Gemini.

**Método:** ejecución del prompt original, evaluación mediante seis criterios y posterior instrucción de corrección.

### Primera ejecución

| Criterio | Resultado |
|---|---|
| Identificación de las seis tareas | Cumplido |
| Clasificación de automatizaciones | Cumplido |
| Priorización de tres oportunidades | Cumplido |
| Diferenciación entre IA y automatizaciones por reglas | Cumplido |
| Reconocimiento de limitaciones técnicas | Cumplido |
| Propuesta de dos indicadores medibles | No cumplido |

**Resultado inicial: 5/6 criterios.**

La respuesta identificó oportunidades de automatización, pero omitió los dos indicadores necesarios para evaluar las mejoras.

También incluyó afirmaciones demasiado categóricas sobre la eliminación de errores manuales.

### Segunda iteración

Se solicitó al modelo revisar su respuesta, incorporar los indicadores faltantes y corregir afirmaciones que no estuvieran suficientemente fundamentadas.

Gemini agregó:

**KPI 1 — Tiempo promedio de procesamiento por pedido**

- Mide el tiempo transcurrido durante la gestión de cada pedido.
- Se calcula dividiendo el tiempo total registrado entre la cantidad de pedidos procesados.
- Permite comparar el proceso manual con el automatizado.

**KPI 2 — Tasa de errores de carga**

- Mide la proporción de pedidos registrados con información incorrecta.
- Se calcula dividiendo los pedidos con errores por el total procesado y multiplicando por 100.
- Permite evaluar si la automatización disminuye las discrepancias de información.

También reconoció que las automatizaciones pueden reducir errores, pero no eliminarlos completamente.

Se identificaron limitaciones relacionadas con el acceso autorizado a WhatsApp, los permisos de Google Sheets y la estabilidad de las integraciones.

**Resultado de la segunda iteración: 6/6 criterios cumplidos considerando ambas respuestas.**

## 5. Resultado obtenido

La IA recomendó comenzar por:

1. Organizar los datos de productos, precios y existencias.
2. Automatizar el registro de pedidos previamente estructurados.
3. Implementar alertas de stock mínimo.

Estas recomendaciones priorizan la calidad de los datos y las automatizaciones basadas en reglas antes de incorporar IA conversacional.

## 6. Limitaciones

El análisis se realizó sobre una empresa ficticia.

No se implementaron las integraciones propuestas ni se midieron ahorros reales de tiempo o reducciones de errores.

Los indicadores constituyen una propuesta de medición y no resultados observados.

Además, el tiempo transcurrido entre la recepción y confirmación de un pedido no necesariamente representa el tiempo efectivo de trabajo.

## 7. Conclusiones

La prueba inicial cumplió cinco de los seis requisitos solicitados.

Mediante una segunda instrucción, fue posible identificar y corregir la omisión, obteniendo una respuesta que cumplió todos los criterios definidos.

**Aprendizaje principal:** un prompt puede mejorarse mediante iteraciones, utilizando criterios de validación para detectar omisiones y solicitar correcciones concretas.

También se comprobó la importancia de distinguir las automatizaciones basadas en reglas de aquellas que realmente necesitan Inteligencia Artificial.

**Estado:** validación del análisis superada mediante dos iteraciones. Implementación técnica pendiente.
