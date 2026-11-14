---
author: Rikelvi Capellán
category: Inteligencia Artificial
cover: /articles/covers/ia-2026-avances-problemas.png
description: "Qué ha mejorado de verdad en la IA este 2026 —modelos, agentes, ciencia— y qué riesgos ya son estructurales: seguridad, desinformación, energía, concentración de poder y la recta final del AI Act."
lang: es
pageTitle: ia-2026-avances-problemas
tags:
  - inteligencia artificial
  - agentes
  - seguridad
  - ai act
  - energía
  - "2026"
  - análisis
timestamp: 14/Nov/2026
title: "IA en 2026: avances reales y los problemas que ya no se pueden ignorar"
translationKey: ai-2026
---

Durante años, la conversación sobre inteligencia artificial iba por delante de la realidad: promesas de agentes autónomos, modelos que iban a reescribir industrias enteras y una carrera por demostrar quién tenía la demo más impresionante. En noviembre de 2026 el tono es otro. La IA ya no está en el escenario: está en el correo, en el calendario, en el buscador y en la cadena de suministro. Y con eso, los fallos también dejaron de ser teóricos.

Este es un repaso a lo que de verdad ha avanzado este año y a las grietas que ya son estructurales. No es una lista de titulares: es un intento de separar capacidad demostrada de riesgo operativo, con las referencias para que puedas verificarlo tú mismo.

## Lo que de verdad ha avanzado

### Modelos que ya razonan por partes

El 12 de noviembre Google presentó **Gemini 4 Hydrogen**, que según la compañía es su mayor actualización de Search hasta la fecha. El cambio interesante no es tanto una puntuación más alta en un benchmark, sino el tipo de tarea que aborda: preguntas con varias partes, errores de escritura difíciles de interpretar y peticiones muy específicas. El modelo descompone la pregunta, consulta simultáneamente varios subtemas y devuelve más enlaces, tablas, gráficos y mapas. También añade un nivel de razonamiento `xhigh` para los casos que lo necesitan.

Que un modelo de este tipo sea el predeterminado en AI Mode y en las preguntas difíciles de AI Overviews dice mucho de hacia dónde va la búsqueda: menos "diez enlaces azules" y más una respuesta construida, con fuentes que el usuario tendría que revisar. Es útil. También traslada al usuario una responsabilidad nueva: comprobar si la respuesta y sus fuentes resisten.

### Agentes que hacen trabajo, no solo conversación

El segundo avance real es la entrada de los agentes en tareas cotidianas. **Claude Duet**, el agente de Anthropic para consumidores, se conecta al correo, al calendario, a Google Docs y a Slack. En una prueba de una semana, _The Verge_ lo describe como un asistente útil para detectar contradicciones entre una reunión y un mensaje directo, o para avisar de un plazo que se había pasado por alto. También como un compañero un poco neurótico: confundió el contexto de un plazo, no captó el tono de un mensaje y llegó a ofrecerse a revisar su propio trabajo.

Ese matiz importa. La ventaja de un agente no es que "piense" mejor que un modelo de chat, sino que tiene acceso a más contexto y puede actuar sobre él. El riesgo tampoco es abstracto: cuanto más contexto y más permisos, más daño puede hacer un error de criterio. La conclusión práctica de la reseña es la correcta: un agente sirve como red de seguridad para tus sistemas de organización, no como sustituto de ellos.

### Ciencia: acelerar la búsqueda, no saltarse la validación

En el terreno científico también hay señales interesantes. Google DeepMind presentó **AlphaGenome 2**, orientado a entender la regulación genética y las raíces celulares de enfermedades. Y un grupo de agentes de IA fue presentado como el descubridor de un yacimiento maya a partir de datos LIDAR de la NASA. La segunda historia es especialmente instructiva: el hallazgo ya había sido publicado años antes por un arqueólogo, y la IA había vuelto a encontrar algo que ya estaba en la literatura.

No es un fracaso de la IA: es exactamente lo que hace bien, buscar patrones a escala. El fracaso sería creer que un resultado generado por un agente sustituye el trabajo de campo, la revisión por pares o el conocimiento previo de una disciplina. La IA acelera la búsqueda; la validación sigue siendo humana.

## Las grietas que ya no son teóricas

### 1. Seguridad: el enlace compartido como agujero

El caso más claro del año es el de **Grok Build**, el agente de programación de SpaceXSI. Un investigador de la firma Claroc encontró 43.601 enlaces de aplicaciones creadas con la herramienta. Más de 35.000 —casi el 95 %— abrían la aplicación y todos sus datos a cualquiera que tuviera el enlace. Entre los datos expuestos había exámenes médicos de 3.784 trabajadores, currículums internos, presupuestos de clientes, planes de ventas y hasta 24 aplicaciones de la propia SpaceXSI con información confidencial.

La causa técnica es sencilla y vergonzosa: el identificador aleatorio del enlace estaba en el subdominio, no en la ruta. Eso permite enumerarlos con servicios de DNS pasivo. Meta tuvo un problema parecido con Muse semanas antes. Y no es un fallo exclusivo de una herramienta: Lovable, Bolt y Replit también generan aplicaciones con direcciones propias, así que el mismo patrón puede repetirse.

La lección no es "no uses agentes para programar". Es que **compartir es una decisión de autorización**, no un detalle de interfaz. Un enlace "solo para quien lo tenga" es una credencial. Si tu producto genera enlaces, necesita autenticación real, permisos por recurso, caducidad y registro de accesos.

### 2. Confianza: respuestas que recomiendan estafas

Otro problema que dejó de ser hipotético es el de las recomendaciones. Un estudio de la firma Podqi analizó 6.795 respuestas de ChatGPT, Gemini y Perplexity a preguntas de compra sobre 151 marcas. En hasta un 15 % de las respuestas de Perplexity aparecían sitios "de riesgo": tiendas falsas que suplantaban a la marca, dominios antiguos reactivados o páginas muertas que alguien podía comprar. ChatGPT quedó en un 8 % y Gemini en un 4 %.

El dato más incómodo es que los modelos a veces inventaban webs regionales para marcas que no tienen presencia regional. Para el usuario, el riesgo es directo: introducir datos de pago en una tienda que parece oficial porque el chatbot la citó. Para la marca, es un problema de reputación y de fraude. Y para quien construye productos con IA, es una señal de que la calidad de una respuesta no se mide solo por lo convincente que suena, sino por la procedencia de sus fuentes.

### 3. Economía: concentración y gobernanza

La semana del 12 de noviembre fue un recordatorio de hasta qué punto la industria depende de unas pocas piezas. Nvidia, el proveedor de chips que sostiene buena parte del despliegue de IA, anunció la dimisión de su CEO, Jensen Huang, después de dos relaciones extramatrimoniales —una con una persona señalada como presunta espía china— y de una investigación del consejo. La CFO, Colette Kress, asumió el cargo de forma interina. La compañía tenía además una cartera de inversiones de unos 99.000 millones de dólares en empresas de IA, desde laboratorios hasta proveedores de nube.

Ese mismo fin de semana, Anthropic confirmó que planea empezar a cotizar el 19 de noviembre, con un precio orientativo de entre 70 y 78 dólares por acción y una valoración de hasta 1,4 billones de dólares.

No hace falta decidir si esto es una burbuja para ver el riesgo: cuando el proveedor de infraestructura también invierte en sus clientes, y los clientes se valoran por lo que pueden comprar con esa infraestructura, la gobernanza de una sola empresa se convierte en un asunto sistémico. La pregunta ya no es solo "¿qué modelo es mejor?", sino "¿quién controla el acceso, el precio y las condiciones?".

### 4. Energía y territorio

La IA consume electricidad, y cada vez más. El informe _Energy and AI_ de la Agencia Internacional de la Energía estimaba que el consumo eléctrico de los centros de datos podría algo más que duplicarse hasta unas 945 TWh en 2030, frente a unas 415 TWh en 2024. No es un problema solo de emisiones: es de red, de precio y de territorio.

En Estados Unidos, la oposición a los centros de datos se convirtió en un tema electoral en las elecciones de medio mandato de 2026. Los votantes apoyaron límites en casi todas las medidas que se votaron, y los grupos críticos ya están presionando para que los políticos cumplan lo prometido. Traducido: construir un centro de datos ya no es solo una decisión técnica o financiera; es una decisión política local.

### 5. Regulación: el AI Act ya no es un borrador

El **Reglamento Europeo de IA** terminó su despliegue principal el 2 de agosto de 2026: desde esa fecha se aplica el grueso de sus obligaciones, con excepciones para los sistemas de alto riesgo, que llegan el 2 de diciembre de 2027 (Anexo III) y el 2 de agosto de 2028 (Anexo I). Además, los sistemas que generan audio, imagen, vídeo o texto sintético y ya estaban en el mercado tienen hasta el 2 de diciembre de 2026 para cumplir las obligaciones de transparencia del artículo 50. Ese mismo día entran en vigor las prohibiciones sobre imágenes íntimas no consentidas y material de abuso sexual infantil.

Para una pyme, esto se traduce en cuatro tareas concretas: clasificar el sistema según su riesgo, documentar las decisiones, etiquetar el contenido sintético cuando corresponda y formar al equipo que lo usa. No es papeleo opcional: es la diferencia entre poder vender en Europa y no poder hacerlo.

### 6. Trabajo y criterio

La IA generativa sigue entrando en los flujos de trabajo creativos. La encuesta del Festival de Gaming de la GDC de este año mostró que más desarrolladores de videojuegos la usan, en un contexto de despidos y presión por producir más rápido. Pero el caso de Grok Build deja una lección más incómoda para el discurso de la productividad: si nadie revisa lo que genera el agente, el ahorro de tiempo se paga después en incidentes.

El patrón que veo en los equipos que funcionan no es "la IA hace el trabajo". Es "la IA hace la primera versión y una persona decide qué se queda". Eso exige criterio, y el criterio es justo lo que no se delega. Como contaba en [mi experiencia con el desarrollo asistido por IA](/articles/desarrollo-asistido-por-ia), la regla sigue siendo la misma: si no puedes explicar una línea, no la fusiones.

## Qué hacer si construyes con IA

Si estás integrando modelos o agentes en un producto, estos son los controles que separan una demo de un sistema:

- **Trata la salida del modelo como entrada no confiable.** Nunca la concatenes directamente en SQL, shell o HTML. Valida, escapa y limita.
- **Define permisos por herramienta, no por agente.** Un agente que puede leer el correo no debería poder enviar dinero. Usa listas de permitidos y aprobación humana para acciones irreversibles.
- **Diseña el intercambio de enlaces como autenticación.** Enlaces privados por defecto, permisos por recurso, caducidad y auditoría. La entropía no sustituye a la autorización.
- **Verifica las fuentes.** Si tu producto recomienda productos, médicos o trámites, limita las respuestas a dominios de confianza y muestra siempre la cita. Un enlace no es una garantía.
- **Mide coste, latencia y energía.** No todos los problemas necesitan el modelo más grande. Enrutar tareas simples a modelos pequeños es una decisión de producto y de sostenibilidad.
- **Prepara el calendario regulatorio.** Clasificación de riesgo, documentación, transparencia y formación. El AI Act ya está aquí, no en un futuro hipotético.
- **Ten un plan de incidentes.** Qué haces si un agente filtra datos, si una recomendación resulta fraudulenta o si un modelo empieza a fallar en producción. Sin ese plan, no hay sistema: hay una apuesta.

## La conclusión incómoda

La IA de 2026 es, a la vez, más capaz y más frágil de lo que sugiere su marketing. Los modelos razonan mejor, los agentes tienen más contexto y la ciencia avanza. Pero los fallos ya no ocurren en un laboratorio: ocurren en un enlace compartido, en una recomendación de compra, en la dimisión de un CEO o en la factura eléctrica de una región.

El cuello de botella ya no es la capacidad del modelo. Es la confianza, la gobernanza y la responsabilidad. Y esas tres cosas no se resuelven con una actualización de pesos: se resuelven con diseño, auditoría y decisiones humanas.

Si un sistema recomienda, compra o decide, necesita las mismas garantías que cualquier otro sistema que hace eso. Esa es la conversación que la industria lleva demasiado tiempo aplazando.

## Referencias

- [EU Artificial Intelligence Act — Implementation Timeline](https://artificialintelligenceact.eu/implementation-timeline/) (actualizado el 31 de agosto de 2026).
- [IEA — Energy and AI](https://www.iea.org/reports/energy-and-ai) (10 de abril de 2025) y [Key Questions on Energy and AI](https://www.iea.org/reports/key-questions-on-energy-and-ai) (16 de abril de 2026).
- [The Verge — Google's new Gemini model is better at understanding complicated questions](https://www.theverge.com/ai-artificial-intelligence/1032505/google-search-ai-mode-gemini-4-hydrogen) (12 de noviembre de 2026).
- [The Verge — Claude's Duet agent is a little neurotic and surprisingly helpful](https://www.theverge.com/ai-artificial-intelligence/1032518/claude-duet-ai-agent-hands-on) (13 de noviembre de 2026).
- [Ars Technica — Grok Build coding agent leaks oodles of confidential info](https://arstechnica.com/security/2026/11/grok-build-coding-agent-leaks-oodles-of-confidential-info-some-belonging-to-spacexsi/) (10 de noviembre de 2026).
- [The Verge — AI chatbots are recommending fake retail websites, study finds](https://www.theverge.com/ai-artificial-intelligence/1032020/gemini-chatgpt-perplexity-shopping-test-risky-fake-websites-citations) (12 de noviembre de 2026).
- [The Verge — Nvidia CEO Jensen Huang resigns amid spy, affair scandals](https://www.theverge.com/ai-artificial-intelligence/1031689/jensen-huang-nvidia-ceo-resigns) (12 de noviembre de 2026).
- [The Verge — Anthropic confirms its IPO plans](https://www.theverge.com/ai-artificial-intelligence/1031894/anthropic-confirms-its-planning-for-its-shares-to-start-publicly-trading-on-november-19th) (12 de noviembre de 2026).
- [The Verge — Data center opponents are cheering midterm results](https://www.theverge.com/policy/1026365/data-centers-midterms-results) (11 de noviembre de 2026).
- [The Verge — Google's AlphaGenome 2 zooms in on the cellular roots of disease](https://www.theverge.com/ai-artificial-intelligence/1031524/google-deepmind-alphagenome-2-genetic-ai-model) (11 de noviembre de 2026).
- [The Verge — No, AI agents did not discover a previously unknown Maya site](https://www.theverge.com/ai-artificial-intelligence/1032125/ai-agents-maya-site-archeology-discovery) (12 de noviembre de 2026).
- [The Verge — More game developers are starting to use generative AI](https://www.theverge.com/games/1032085/gdc-festival-of-gaming-annual-survey-ai-layoffs) (12 de noviembre de 2026).
