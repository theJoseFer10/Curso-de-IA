# Entregable: Bosquejo de flujo funcional con IA

**Nombre:** Jose Fernando Arenas Camacho
## 1. Descripción del micro-producto o flujo

**Nombre del flujo:** Clasificación y Formalización Automática de Reportes Urbanos.

**Contexto:** Este flujo se activa cuando un ciudadano envía una queja sobre la infraestructura pública a través de la aplicación móvil. El objetivo es eliminar el "ruido" de las quejas informales y entregar a las autoridades un documento técnico listo para su atención.

Pasos del flujo:

- Entrada: El ciudadano sube una descripción breve y una fotografía del desperfecto desde su ubicación.

- Procesamiento (IA): El sistema analiza el texto del ciudadano para identificar el tipo de problema, la gravedad y la urgencia.

- Estandarización: La IA redacta un reporte formal siguiendo el protocolo administrativo municipal.

- Salida: El reporte se envía automáticamente al departamento correspondiente (Obras Públicas, Alumbrado, Agua, etc.) y se le asigna un número de folio al ciudadano.

## 2. Uso puntual de la IA

**¿En qué paso interviene?:** En el Paso 2 y 3 (Análisis y Redacción).

Tarea que realiza: La IA actúa como un filtro inteligente que traduce lenguaje ciudadano (informal) a lenguaje administrativo (formal) y decide a qué dependencia pertenece el caso para evitar errores de envío.

Ejemplo de Prompt:

    "Actúa como un Asistente de Gestión Urbana. Analiza el siguiente mensaje de un ciudadano: '[MENSAJE_CIUDADANO]'. Identifica la categoría del problema (Bache, Fuga, Alumbrado, Limpieza) y redacta un reporte técnico de máximo 3 párrafos para el ayuntamiento. Determina la urgencia como Alta si hay riesgo de accidentes, o Media en otros casos. Devuelve el resultado en formato JSON."

## 3. Reflexión.

**¿Qué me facilitó imaginar este flujo con IA en lugar de hacerlo manual?**
Me permitió ver que la IA puede actuar como un "empleado administrativo virtual" que trabaja 24/7. Hacer esto de forma manual requeriría que una persona leyera cada mensaje y lo clasificara, lo cual es lento y propenso a errores humanos; la IA automatiza la parte más pesada del proceso: el análisis inicial.