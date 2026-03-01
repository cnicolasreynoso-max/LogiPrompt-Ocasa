LogiPrompt Ocasa: Eficiencia Documental y Operativa mediante Fast Prompting
Introducción
Nombre del Proyecto: LogiPrompt Ocasa

Alumno: Christian Reynoso

Comisión: 95825

Este proyecto desarrolla una Prueba de Concepto (POC) para solucionar fallas críticas en la logística de "última milla". Se enfoca en digitalizar reportes de incidentes de choferes (especialmente en el interior) y asegurar el cumplimiento del protocolo de custodia de remitos en cabina.

Presentación del Problema
En la operación diaria de transporte para clientes como Molinos, existen tres dolores principales:

Falta de datos: Los choferes no informan por qué falló una visita (turnos no dados, avisos no conseguidos), perdiendo trazabilidad.

Pérdida de Remitos: Los documentos se quedan en los pallets o pedidos, cuando el protocolo exige que viajen en la cabina con el chofer.

Barrera Operativa: El personal de conducción no tiene tiempo para usar apps complejas; necesitan soluciones vía lenguaje natural (texto/audio).

Objetivos
Automatizar la clasificación de incidentes logísticos usando IA.

Validar el cumplimiento de protocolos internos mediante análisis de texto.

Generar material visual de capacitación de forma rápida con IA generativa.

Metodología
Se implementa un flujo de trabajo donde el mensaje informal del chofer es procesado por un modelo de lenguaje. Se utiliza una metodología de refinamiento iterativo, probando los prompts en entornos reales para asegurar que la IA comprenda la jerga logística argentina.

Herramientas y Tecnologías
Técnicas de Prompting: Zero-shot (clasificación rápida), One-shot y Few-shot (para contexto específico de Ocasa).

Implementación: Python en Jupyter Notebook (Google Colab).

Modelos de IA: OpenAI API (GPT-3.5/4) y Nightcafe (para generación de imágenes de señalética y capacitación).

Justificación de Viabilidad
El proyecto es viable porque utiliza recursos de bajo costo (API Keys) y tecnologías que no requieren infraestructura nueva. La rentabilidad se justifica al reducir las devoluciones de mercadería por falta de documentación, cuyo costo es infinitamente mayor al de una consulta a la IA.
Few-shot: Para entrenar al modelo en el reconocimiento de la jerga logística local y códigos de incidente específicos de Ocasa.

Modelos de Lenguaje: OpenAI API (GPT) a través de una Jupyter Notebook en Python.

Modelos de Imagen: Stable Diffusion / Nightcafe para generar material de capacitación visual.

### Implementación Técnica (POC)
Para esta Prueba de Concepto, se ha desarrollado una Notebook interactiva. 

**Nota sobre la API:** Debido a limitaciones de cuota en la API de OpenAI, la Notebook actual utiliza una **función de simulación (Mocking)**. Esta función replica exactamente la lógica de clasificación que se obtuvo durante las pruebas reales con el modelo `gpt-3.5-turbo`, permitiendo al tutor evaluar la estructura de los prompts y la salida de datos sin necesidad de configurar una API Key de pago.

**Técnicas utilizadas:**
* **Role Prompting:** Se define el perfil de Analista de CX.
* **Few-Shot Prompting:** Se integraron ejemplos de jerga logística para asegurar que la IA interprete correctamente las fallas en el interior.

"Se incluye material visual generado mediante IA (Nightcafe) para reforzar el protocolo de remitos en cabina, atacando la problemática de pérdida de documentación."
