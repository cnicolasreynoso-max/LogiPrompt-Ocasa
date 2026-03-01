LogiPrompt Ocasa: Inteligencia Artificial para la Gestión de Última Milla
Introducción
Nombre del Proyecto: LogiPrompt Ocasa

Autor: Christian Reynoso

Comisión: 95825

Presentación del Problema
En las operaciones logísticas de distribución (específicamente para clientes como Molinos), se detectan tres fallas críticas:

Sub-notificación de incidentes: Los choferes en el interior no reportan motivos específicos de falla (turnos no asignados, avisos fallidos) por la complejidad de los sistemas actuales.

Pérdida de documentación: Incumplimiento del protocolo de custodia de remitos (deben estar en cabina, pero suelen perderse en los pallets).

Barrera técnica: Los choferes operan en movilidad y con poco tiempo, dificultando la carga de datos manual.

Relevancia: Resolver esto permite al equipo de CX transformar "visitas no realizadas" en datos accionables para mejorar el ruteo y la relación con el cliente.

Objetivos del Proyecto
General: Desarrollar una Prueba de Concepto (POC) que automatice la clasificación de reportes logísticos mediante IA.

Específicos: * Implementar técnicas de Fast Prompting para extraer datos de mensajes informales.

Crear una herramienta de concientización visual mediante modelos de Texto-a-Imagen.

Asegurar la rentabilidad de la solución minimizando las consultas a la API.

Metodología
El proyecto se desarrolla bajo una metodología de Procesamiento de Lenguaje Natural (NLP) asistido. Se capturan las transcripciones de mensajes de voz de los choferes y se pasan por un motor de IA (GPT-4o/3.5) configurado con un System Prompt robusto que actúa como un Analista de Operaciones Senior. Se utiliza un enfoque iterativo para refinar los resultados basándose en casos reales de la operación de Ocasa.

Herramientas y Tecnologías
Técnicas de Prompting: * Zero-shot: Para clasificar urgencias de forma rápida.

Few-shot: Para entrenar al modelo en el reconocimiento de la jerga logística local y códigos de incidente específicos de Ocasa.

Modelos de Lenguaje: OpenAI API (GPT) a través de una Jupyter Notebook en Python.

Modelos de Imagen: Stable Diffusion / Nightcafe para generar material de capacitación visual.
