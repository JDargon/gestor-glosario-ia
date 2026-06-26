# Glosario de inteligencia artificial

## Agente de IA

Sistema basado en inteligencia artificial que puede tomar decisiones y realizar acciones usando herramientas. Por ejemplo, puede leer archivos, consultar documentación, ejecutar comandos o modificar código.

## Arnés / harness

En IA, un harness es la “estructura de trabajo” que rodea al modelo para que pueda hacer tareas de forma útil y controlada. Incluye instrucciones, herramientas disponibles, memoria, permisos, control de errores, pruebas y formas de ejecutar acciones. No es el modelo en sí, sino el entorno que lo guía y lo conecta con el mundo exterior.

Por ejemplo, un agente que puede leer archivos, usar una terminal, consultar una API y comprobar resultados necesita un harness que organice todo ese proceso.

## Autoprompting / generación automática de prompts

Técnica en la que un sistema de IA genera, ajusta o mejora prompts de forma automática o semiautomática para conseguir mejores resultados en una tarea.

Puede usarse para transformar una petición general en instrucciones más precisas, crear variantes de un prompt, adaptar el formato de salida o preparar indicaciones para otros modelos o agentes. Está relacionado con el metaprompting, pero pone más énfasis en la automatización del proceso.

## Benchmark

Prueba comparativa que sirve para medir el rendimiento de distintos modelos o agentes de IA en una tarea concreta. Un benchmark define un conjunto de casos, condiciones de ejecución y criterios de evaluación para poder comparar resultados de forma objetiva.

## Canvas / lienzo

Espacio de trabajo visual o editable asociado a una conversación con IA, pensado para crear, revisar o modificar contenido de forma más estructurada que en un chat normal.

Un canvas puede usarse para trabajar sobre textos, código, documentos u otros materiales mientras la IA propone cambios, comenta partes concretas o ayuda a reorganizar el contenido.

## Code Interpreter / intérprete de código

Herramienta que permite a un sistema de IA ejecutar código para resolver tareas que requieren cálculo, análisis de datos, transformación de archivos o generación de resultados comprobables.

Por ejemplo, puede usarse para analizar una hoja de cálculo, crear un gráfico, convertir un archivo o comprobar una operación matemática. No es el modelo de IA en sí, sino una herramienta que el modelo puede utilizar cuando la tarea lo requiere.

## Condiciones de ejecución

Conjunto de reglas o límites bajo los que se prueba un modelo o agente: herramientas disponibles, número de intentos, tiempo, coste, permisos, acceso a terminal, acceso a internet y otros recursos.

## Configuración del agente

Forma concreta en la que se prepara un agente para trabajar: qué instrucciones recibe, qué herramientas puede usar, qué memoria tiene, cómo se controla el loop y cómo se valida el resultado.

## Connector / conector

Integración que permite a un sistema de IA acceder a una fuente de información, herramienta, aplicación o servicio externo.

Un conector puede servir para consultar archivos, bases de datos, calendarios, repositorios, gestores de tareas u otras plataformas. Está relacionado con MCP y GPT Actions, pero es un concepto más general: MCP puede funcionar como protocolo para conectar recursos, mientras que una acción de GPT o un conector concreto implementan una forma práctica de acceso.

## Context engineering / ingeniería de contexto

Proceso de preparar y organizar la información que recibe un modelo o agente de IA para que pueda trabajar correctamente. Incluye instrucciones, documentación, estado del proyecto, archivos relevantes, restricciones, herramientas y resultados anteriores.

Una buena ingeniería de contexto ayuda a que el agente tome decisiones más precisas y mantenga la coherencia durante tareas largas.

## Context rot / degradación del contexto

Pérdida progresiva de precisión que puede producirse cuando una conversación o sesión de trabajo acumula demasiada información. El agente puede olvidar requisitos, confundir decisiones anteriores o prestar menos atención a detalles importantes.

Algunos sistemas intentan reducir este problema guardando el estado del proyecto en archivos y dividiendo el trabajo en fases pequeñas.

## Conversation starters / iniciadores de conversación

Frases o preguntas sugeridas que aparecen al empezar a usar un asistente de IA para orientar a la persona usuaria sobre qué puede pedirle.

En un GPT personalizado, los conversation starters ayudan a mostrar ejemplos de uso, aclarar el propósito del asistente y facilitar que la primera interacción sea más concreta.

## Criterios de aceptación

Condiciones concretas que deben cumplirse para considerar que una funcionalidad está correctamente terminada.

Por ejemplo: que un botón quede deshabilitado durante una petición, que se muestre un mensaje de error comprensible o que los datos se actualicen después de registrar una acción. Permiten comprobar de forma objetiva si el agente ha realizado correctamente el trabajo.

## Deep research / investigación profunda

Modo de trabajo de un sistema de IA orientado a investigar una cuestión compleja consultando, comparando y sintetizando información de varias fuentes. A diferencia de una búsqueda rápida, no se limita a encontrar una respuesta inmediata, sino que intenta reunir contexto, analizar distintas fuentes y elaborar una explicación más completa.

El deep research puede ser útil para preparar informes, comparar opciones, estudiar un tema técnico o recopilar información sobre cuestiones que requieren más de una consulta. Aun así, sus resultados deben revisarse, especialmente si se usan para tomar decisiones importantes o si dependen de fuentes externas.

## Embedding / representación vectorial

Representación numérica de un texto, imagen, audio u otro tipo de dato, creada para que un sistema de IA pueda comparar significados de forma matemática.

En modelos de lenguaje, un embedding convierte palabras, frases o documentos en vectores. Los elementos con significados parecidos suelen quedar cerca entre sí en ese espacio vectorial. Por eso los embeddings se usan a menudo en búsquedas semánticas, sistemas RAG, recomendadores y clasificación de contenido.

Por ejemplo, las frases “comprar un coche” y “adquirir un automóvil” pueden tener embeddings similares aunque no usen exactamente las mismas palabras.

## Especificación

Documento o conjunto de instrucciones que describe con precisión qué se quiere construir y cómo debe comportarse. Puede indicar el objetivo, los requisitos, los límites de la tarea, los casos especiales y las condiciones que deben cumplirse para considerar el trabajo terminado.

En el desarrollo asistido por IA, la especificación sirve como fuente de verdad para que el agente no dependa únicamente del historial de la conversación.

## Estado del proyecto

Información que permite saber en qué punto se encuentra un proyecto: fases completadas, tareas pendientes, decisiones tomadas, errores detectados y próximos trabajos previstos.

Los sistemas de desarrollo agéntico suelen guardar este estado en archivos para que el agente pueda continuar el trabajo en futuras sesiones sin depender únicamente de la memoria del chat.

## Evaluación

Proceso mediante el cual se mide el rendimiento de un modelo o agente. En este contexto, la evaluación determina qué porcentaje de tareas consigue resolver correctamente y bajo qué condiciones lo hace.

## Fine-tuning / ajuste fino

Técnica para adaptar un modelo de IA ya entrenado a una tarea, estilo o dominio concreto mediante un entrenamiento adicional con ejemplos específicos.

En lugar de crear un modelo desde cero, se parte de un modelo general y se le proporcionan datos seleccionados para que aprenda determinados comportamientos, formatos de respuesta o conocimientos especializados. Por ejemplo, puede ajustarse un modelo para clasificar documentos, responder con el estilo de una empresa o trabajar mejor con vocabulario técnico de un sector.

El fine-tuning modifica el comportamiento interno del modelo y requiere preparar datos de calidad.

## Fuente de verdad

Referencia principal que se considera válida para conocer los requisitos y decisiones de un proyecto.

En el desarrollo guiado por especificaciones, la fuente de verdad suele ser la especificación escrita, en lugar de depender de mensajes dispersos en un chat o de lo que el agente pueda recordar.

## GPT Actions / acciones de GPT

Funciones que permiten a un GPT personalizado conectarse con servicios externos para consultar información o realizar operaciones fuera de la conversación.

Una acción de GPT puede servir, por ejemplo, para buscar datos en una aplicación, enviar una solicitud a una API, consultar una base de datos o activar un flujo de trabajo. A diferencia del conocimiento cargado en el GPT, las acciones no solo proporcionan contexto estático, sino que permiten interactuar con sistemas externos.

## Grounding / fundamentación en información

Proceso de apoyar las respuestas de un sistema de IA en información concreta, verificable o proporcionada como contexto. Sirve para reducir respuestas inventadas o demasiado generales, haciendo que el modelo se base en documentos, datos, instrucciones o fuentes relevantes para la tarea.

El grounding puede hacerse mediante documentos aportados por el usuario, información recuperada de una base de datos, resultados de búsqueda, contenido de un repositorio o una fuente de verdad del proyecto. Está relacionado con RAG, pero no es lo mismo: RAG es una técnica para recuperar información externa, mientras que grounding es el principio general de basar la respuesta en información de referencia.

## GSD / Get Shit Done / Get Stuff Done

Sistema de trabajo para desarrollar proyectos de software con agentes de IA. Organiza el proceso mediante recopilación de requisitos, planificación, división por fases, gestión del contexto, ejecución de tareas y verificación de resultados.

Intenta que el agente mantenga el rumbo durante proyectos largos, evitando que pierda requisitos importantes o se desvíe de los objetivos iniciales. A diferencia de SDD, que es una metodología centrada en definir primero las especificaciones, GSD plantea un sistema de trabajo más amplio para organizar todo el desarrollo del proyecto.

## Knowledge / conocimiento

Información, documentos o archivos que se proporcionan a un sistema de IA para que los use como referencia al responder o realizar una tarea.

En un GPT personalizado, el conocimiento cargado puede incluir guías, glosarios, manuales, políticas internas u otros materiales aportados por la persona que lo configura. No significa que el modelo haya sido entrenado de nuevo con esos datos, sino que puede consultarlos como contexto durante su funcionamiento.

## Loop / bucle

Un loop es un ciclo repetido de trabajo. En agentes de IA suele seguir una secuencia similar a:

**observar → razonar → actuar → comprobar el resultado → corregir → repetir**

La IA no responde una sola vez, sino que va iterando hasta avanzar en una tarea. En programación con agentes se habla a menudo de bucles tipo ReAct: el modelo razona, usa una herramienta, observa el resultado y vuelve a decidir el siguiente paso.

## MCP / Model Context Protocol

Protocolo que permite conectar modelos o agentes de IA con herramientas, datos y servicios externos de forma estructurada.

MCP actúa como una capa común para que una IA pueda acceder, por ejemplo, a archivos, bases de datos, documentación, APIs o aplicaciones sin necesitar una integración distinta para cada caso. En un sistema agéntico, puede facilitar que el modelo use recursos externos manteniendo reglas claras sobre qué puede consultar o ejecutar.

## Memory / memoria

Capacidad de un sistema de IA para conservar o reutilizar información de interacciones anteriores, preferencias de la persona usuaria, datos de un proyecto o decisiones ya tomadas.

La memoria puede ayudar a mantener continuidad entre sesiones, evitar repeticiones y adaptar mejor las respuestas. No debe confundirse con el contexto inmediato de una conversación: el contexto es la información disponible en ese momento, mientras que la memoria intenta persistir más allá de una interacción concreta.

## Metaprompting

Técnica que consiste en usar instrucciones para generar, mejorar u organizar otros prompts.

En desarrollo agéntico puede emplearse para que la IA convierta una idea general en requisitos, planes de implementación, tareas concretas o instrucciones especializadas para otros agentes.

## Modelo de IA

El “cerebro” principal del sistema. Es el modelo que interpreta instrucciones, genera respuestas, razona y decide qué hacer.

## OpenSpec

Herramienta de código abierto para organizar el desarrollo guiado por especificaciones con asistentes y agentes de programación.

Permite definir propuestas de cambio, requisitos y tareas antes de modificar el código. Las especificaciones pueden guardarse junto al proyecto, de forma que sean revisables, reutilizables y versionables. Su idea principal es acordar primero qué debe cambiar y después realizar la implementación.

OpenSpec no es la metodología en sí, sino una herramienta para aplicar de forma práctica el enfoque SDD.

## Orchestration / orquestación

Proceso de coordinar varios componentes de un sistema de IA para completar una tarea. Puede incluir modelos, agentes, herramientas, memoria, recuperación de información, validaciones y pasos de decisión.

La orquestación define cómo se conectan esas partes, en qué orden actúan y qué ocurre según el resultado de cada paso. Por ejemplo, un sistema puede buscar información, pasarla a un modelo, ejecutar una herramienta y después verificar la respuesta antes de mostrarla.

## Planificación por fases

Forma de dividir un proyecto grande en bloques pequeños y manejables. Cada fase tiene un objetivo concreto, unas tareas determinadas y una forma de comprobar que está terminada.

En programación agéntica, esta división permite dar al agente contextos más claros y reducir la complejidad de cada intervención.

## Programación agéntica

Forma de usar IA en la que el modelo no solo responde con texto o código, sino que actúa como un agente: analiza un problema, usa herramientas, modifica archivos, ejecuta pruebas y corrige errores.

## Proposal / propuesta de cambio

Documento que describe una modificación que se quiere realizar en un proyecto antes de implementarla.

Puede indicar el problema, el objetivo, los requisitos afectados y el comportamiento esperado. En herramientas como OpenSpec, la propuesta ayuda a revisar y aprobar el cambio antes de que el agente empiece a modificar el código.

## Quick search / búsqueda rápida

Consulta breve realizada por un sistema de IA para encontrar información concreta, actual o verificable en poco tiempo. Se utiliza cuando la pregunta requiere una comprobación sencilla, como localizar un dato, confirmar una noticia, consultar una fecha o encontrar una fuente.

La búsqueda rápida se diferencia del deep research en el nivel de profundidad. En una búsqueda rápida, la IA intenta responder de forma directa usando pocas fuentes relevantes. En deep research, la IA dedica más pasos a investigar, comparar, sintetizar y elaborar una respuesta más completa.

## RAG / Retrieval-Augmented Generation / generación aumentada por recuperación

Técnica que permite a un modelo de IA consultar información externa antes de generar una respuesta.

El sistema busca primero contenido relevante en documentos, bases de datos u otras fuentes y después entrega esa información al modelo como contexto. De esta forma, la IA puede responder usando datos concretos, privados o más actualizados sin necesidad de volver a entrenar el modelo.

Por ejemplo, un asistente puede buscar en los manuales de una empresa y utilizar los fragmentos encontrados para contestar una pregunta. En un sistema RAG, el modelo no memoriza necesariamente los documentos, sino que los consulta cuando los necesita.

## Repositorio

Conjunto organizado de archivos de un proyecto de software.

En programación agéntica, el agente puede explorar un repositorio para entender cómo está construido el proyecto antes de hacer cambios.

## SDD / Spec-Driven Development / desarrollo guiado por especificaciones

Metodología de desarrollo de software guiada por especificaciones. Consiste en definir con claridad qué debe hacer una funcionalidad antes de comenzar a programar.

La especificación puede incluir requisitos, comportamiento esperado, restricciones, casos de uso, criterios de aceptación y pruebas. En el desarrollo con IA, ayuda a evitar instrucciones ambiguas y permite que el agente trabaje siguiendo una referencia clara y revisable.

Su flujo habitual es:

**especificar → planificar → implementar → probar → verificar**

El código se crea a partir de requisitos previamente definidos y no solo mediante instrucciones improvisadas durante la conversación. Esto facilita revisar el trabajo, detectar desviaciones y comprobar si la implementación coincide con lo solicitado.

SDD es la metodología general. Herramientas como OpenSpec ayudan a aplicarla, mientras que sistemas como GSD amplían el enfoque con planificación por fases, gestión del contexto, ejecución y verificación.

## Skill / habilidad

Capacidad específica y reutilizable que se añade a un sistema de IA o a un agente para que pueda realizar mejor un tipo de tarea.

Una skill puede incluir instrucciones, ejemplos, reglas, acceso a herramientas o pasos de trabajo reutilizables. Por ejemplo, una IA puede tener una skill para revisar documentos, generar informes, analizar código o transformar archivos siguiendo un formato concreto.

## SWE-Bench Pro

Benchmark usado para evaluar modelos o agentes de IA en tareas de programación.

Mide si la IA es capaz de resolver problemas reales de software, como corregir errores, modificar código o pasar pruebas dentro de un repositorio.

## Tasa de resolución

Porcentaje de tareas que un modelo consigue completar correctamente en un benchmark.

Por ejemplo, decir que un modelo obtiene un 80,3 % significa que resolvió correctamente ese porcentaje de los casos evaluados.

## TDD / Test-Driven Development / desarrollo guiado por pruebas

Metodología de desarrollo de software en la que las pruebas se escriben antes que el código que debe cumplirlas.

Su ciclo habitual es:

**escribir una prueba que falle → implementar el código mínimo para que pase → mejorar o refactorizar el código sin romper la prueba**

Este proceso se conoce como **Red → Green → Refactor**.

En programación con agentes de IA, el TDD permite dar al agente criterios verificables: el agente modifica el código, ejecuta los tests y corrige su solución hasta que las pruebas pasan.

## Tests / pruebas

Comprobaciones automáticas que sirven para verificar si el código funciona correctamente.

En benchmarks de programación, pasar los tests suele ser una señal de que la solución propuesta por la IA es válida.

## Token

Unidad mínima o fragmento de texto que utiliza un modelo de lenguaje para procesar y generar contenido. Un token puede ser una palabra completa, parte de una palabra, un signo de puntuación o un espacio, según el sistema de tokenización usado.

Los modelos no leen el texto exactamente como lo ve una persona, sino dividido en tokens. Por eso los límites de contexto, la longitud de una respuesta y a veces el coste de uso suelen medirse en tokens.

## Tool / herramienta

Recurso que un sistema de IA puede usar para realizar una tarea que no depende solo de generar texto. Una herramienta puede permitir consultar archivos, ejecutar código, buscar información, llamar a una API, modificar documentos o interactuar con una aplicación externa.

En un agente de IA, las herramientas amplían lo que el modelo puede hacer: el modelo decide cuándo usarlas y el sistema ejecuta la acción mediante la herramienta correspondiente.

## Verificación

Proceso de comprobar que el trabajo realizado coincide con los requisitos definidos.

Puede incluir revisión del código, ejecución de tests, comprobación de criterios de aceptación y comparación entre la especificación y el resultado final. En un flujo agéntico, la verificación permite detectar errores y solicitar correcciones antes de considerar terminada una tarea.

## Vibe coding / programación por conversación con IA

Práctica de desarrollo de software en la que una persona construye o modifica código dando instrucciones en lenguaje natural a una herramienta de IA. En lugar de escribir todo el código manualmente desde el principio, la persona describe lo que quiere conseguir, revisa la propuesta generada por la IA y va ajustando el resultado mediante nuevas indicaciones.

El vibe coding puede ser útil para prototipar, explorar ideas o avanzar rápidamente en tareas pequeñas, pero requiere revisión humana. No debe confundirse con la programación agéntica: en el vibe coding la persona suele dirigir la conversación paso a paso, mientras que en la programación agéntica el sistema puede actuar con más autonomía, usar herramientas, modificar archivos y comprobar resultados.

Por ejemplo, una persona puede pedir a la IA que cree una pantalla de login, revisar el código generado, pedir cambios en los estilos y después corregir errores detectados durante la prueba.

## Workflow / flujo de trabajo

Secuencia organizada de pasos que se siguen para completar una tarea o proyecto.

En SDD puede ser:

**especificar → planificar → implementar → probar → verificar**

En sistemas como GSD, el flujo también puede incluir recopilación de requisitos, creación de una hoja de ruta, división por fases y actualización del estado del proyecto.