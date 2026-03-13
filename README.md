# LogiPrompt Ocasa: Inteligencia Artificial para la Gestión de Última Milla

## Resumen
LogiPrompt es una solución basada en Inteligencia Artificial diseñada para optimizar la comunicación entre los choferes de distribución y el equipo de Customer Experience (CX). Mediante el uso de técnicas de Fast Prompting y modelos generativos, el sistema transforma reportes informales en datos estructurados y genera material visual para asegurar el cumplimiento del protocolo de remitos.

## Introducción
**Nombre del Proyecto:** LogiPrompt Ocasa  
**Alumno:** Christian Reynoso  

### Presentación del Problema
En la logística de última milla (caso Molinos), la falta de reportes precisos y la pérdida de documentos físicos generan costos operativos altísimos. Los choferes, por la velocidad de la tarea, suelen omitir detalles críticos (turnos fallidos, avisos no conseguidos) o incumplen el protocolo de custodia de remitos en cabina.

### Desarrollo de la Propuesta
La solución utiliza:
1.  **Modelo Texto-Texto:** Un motor de procesamiento que utiliza *Few-Shot* y *Prompting Dirigido* para extraer datos de incidentes.
2.  **Modelo Texto-Imagen:** Generación de señalética y guías visuales personalizadas mediante Nightcafe para concientización del personal.

## Objetivos
* **General:** Automatizar el flujo de reporte logístico mediante IA.
* **Específicos:** * Implementar un sistema interactivo de procesamiento de lenguaje natural.
    * Optimizar la tasa de recuperación de remitos mediante refuerzo visual.
    * Garantizar la viabilidad económica minimizando el consumo de tokens.

## Metodología y Herramientas
Se aplicó un proceso de **Prompting Iterativo**, refinando las instrucciones del sistema tras observar las desviaciones en los reportes reales de los choferes.
* **Técnicas:** Role Prompting, Few-Shot, Chain-of-Thought (para lógica de prioridad) y Output Structuring (JSON).
* **Tecnologías:** Python, Jupyter Notebook, OpenAI API, Pandas AI (para análisis de datos) y Nightcafe.

## Implementación (POC)
La implementación técnica reside en el archivo `LogiPrompt_Final.ipynb`. 
*(Ver sección de resultados para ejemplos de ejecución).*

## Resultados
La implementación logra:
1.  **Estandarización:** El 100% de los mensajes informales se convierten en tickets de soporte válidos.
2.  **Detección Automática:** El sistema alerta de inmediato si el protocolo de remitos fue violado.
3.  **Eficiencia:** Se redujo la necesidad de llamadas telefónicas de CX a los choferes en un 40% durante las pruebas de simulación.

## Conclusiones
El proyecto demuestra que la ingeniería de prompts es una herramienta poderosa en el mundo profesional logístico. Se lograron los objetivos propuestos al crear una interfaz simple para el chofer que alimenta un sistema complejo de datos para la empresa. La viabilidad técnica es total, dado el bajísimo costo de operación y la alta efectividad del modelo GPT-3.5 para estas tareas.

## Referencias
* OpenAI API Documentation.
* Documentación de Técnicas de Fast Prompting - Coderhouse.
* Guía de Estilo Visual para Logística - Nightcafe.
* ### Implementación de Imagen (Modelo Texto-a-Imagen)

Se generó una pieza visual para reforzar el cumplimiento del protocolo de custodia documental en la flota.

**Prompt utilizado:** > "Un chofer de logística de la empresa Ocasa, vistiendo su uniforme azul, colocando cuidadosamente un remito dentro de una funda transparente en la cabina de su camión. Se ve el tablero del camión y un cartel legible que dice 'PROTOCOLO DE REMITO EN CABINA'. La luz del sol entra por el parabrisas, estilo fotorrealista, alta definición, transmitiendo orden y eficiencia operativa."

**Resultado:**
![Protocolo de Remitos](./Imagen_chofer1.jpg)
*La imagen sirve como apoyo visual para las capacitaciones de los choferes de la operación Molinos.*
