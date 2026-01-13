# Proyecto Integrador: Tu Micro-Producto con IA

**Nombre: Jose Fernando Arenas Camacho**

## 1: Problema y Contexto.

En muchos municipios, la comunicación entre ciudadanos y autoridades es ineficiente. Los ciudadanos detectan baches, fugas de agua o fallas en el alumbrado, pero no saben cómo reportarlos formalmente o sus quejas son ignoradas por falta de claridad técnica. Esto causa que los problemas urbanos persistan, afectando la calidad de vida. Actualmente, los reportes son desordenados y difíciles de procesar manualmente. Usando IA, podemos transformar estas quejas casuales en datos estructurados y técnicos que las autoridades puedan atender de inmediato, mejorando la respuesta gubernamental.

## 2: Solución Propuesta.

Mi micro-producto es CivicFix, un asistente inteligente que actúa como puente entre el ciudadano y el ayuntamiento. El flujo funciona así:

- Entrada: El ciudadano describe el problema en lenguaje natural (ej. "Hay un hoyo enorme en mi calle") y sube una foto.

- Procesamiento IA: Un asistente personalizado (Custom GPT) analiza el texto y la imagen para clasificar el incidente, evaluar la urgencia y extraer la ubicación.

- Salida: La IA genera un reporte técnico formal y lo organiza en una base de datos para generar visualizaciones que ayuden a los tomadores de decisiones a ver tendencias (como el aumento de baches en lluvias).

- Experiencia del Usuario: El ciudadano recibe un folio de seguimiento y la satisfacción de que su reporte fue redactado profesionalmente y enviado al departamento correcto.

## 3: Parte Técnica.

La arquitectura de CivicFix se basa en tres componentes:

- Asistente Personalizado: Un modelo de lenguaje (como ChatGPT) configurado con un System Prompt de analista urbano.

- Workflow: Un flujo de 3 pasos (Captura → Clasificación por IA → Registro en Hoja de Cálculo/Base de Datos).

- Análisis de Datos: Uso de herramientas de visualización para detectar patrones temporales.

Prompt Clave (Control de Clasificación):

    "Actúa como un Ingeniero de Obra Pública. Tu tarea es analizar el reporte del usuario: '[REPORTE]'. Clasifícalo en una de estas categorías: Pavimentación, Alumbrado o Fuga de Agua. Redacta una descripción técnica inmutable, sin juicios de valor y con lenguaje profesional. Si el reporte implica peligro inmediato (ej. cables expuestos), marca la urgencia como 'CRÍTICA'. Formatea la salida como una lista: Categoría, Descripción, Urgencia."

## 4. Reflexión Final

A lo largo de este curso, aprendí que diseñar un asistente no es solo "dar una orden", sino estructurar un pensamiento. Me sorprendió cómo técnicas como el Chain of Thought y el Step-back pueden evitar que la IA cometa errores de lógica en procesos críticos como la gestión urbana. En una segunda versión, mejoraría la integración directa con mapas GPS para que la ubicación no dependa solo del texto del usuario. Este proceso me dio la autonomía para pasar de ser un usuario de IA a ser un diseñador de soluciones.
Evidencia para tu archivo adjunto (Google Drive / GitHub)

Como el entregable pide una evidencia (imagen o esquema), te sugiero crear un archivo llamado evidencia_proyecto.pdf o una carpeta en GitHub que contenga:

- Diagrama de Flujo: Un dibujo simple de los pasos (puedes hacerlo en Canva o a mano y tomarle foto).

- Captura de Pantalla: Una simulación de un chat donde el usuario da una queja y la IA responde con el reporte técnico que diseñamos en la Lección 6.

- JSON de Workflow (Opcional): El texto del prompt estructurado que pusimos arriba.