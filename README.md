# Titulo

## 📌 Descripción del Proyecto

Este proyecto aplica técnicas de **procesamiento de lenguaje natural (NLP)** y **modelos generativos** al análisis económico, específicamente al estudio del comercio internacional utilizando el modelo de gravedad. Se desarrolla un asistente económico capaz de interpretar consultas sobre exportaciones, distancias, PIB, acuerdos comerciales, entre otros factores, integrando componentes de machine learning, análisis de datos y retrieval-augmented generation (RAG).

---

## 🎯 Objetivo del Proyecto

Desarrollar una solución basada en IA que permita analizar, predecir y explicar dinámicas del comercio bilateral entre países utilizando datos reales y modelos generativos. El sistema debe responder preguntas del usuario, hacer análisis de datos y generar predicciones usando una interfaz amigable.

---

## 📊 Descripción del Dataset

🔗 **Fuente** : Clase comercio internacional, Universidad de los Andes


**Descripción**: El dataset utilizado en este proyecto proviene de una clase de Comercio Internacional y contiene información estructurada para aplicar modelos de gravedad comercial, los cuales se utilizan comúnmente para explicar los flujos comerciales entre países.

Incluye transacciones bilaterales entre países correspondientes al período 2021–2023, y contempla variables económicas relevantes como el Producto Interno Bruto (PIB) de los países involucrados, los niveles arancelarios y los tipos de relación comercial y diplomática.

La base contiene 55.559 observaciones y 12 variables, almacenadas en un archivo .csv con valores monetarios expresados en dólares estadounidenses (USD).

 
### 📌 Variables del dataset

- `Año`: Año del registro (2021).
- `Importador` y `Exportador`: Países involucrados en la transacción.
- `Exports`: Valor de las exportaciones en dólares.
- `Distancia`: Distancia geográfica entre capitales.
- `PIBorigen`: PIB del país exportador.
- `PIBdestino`: PIB del país importador.
- `Arancel`: Porcentaje de arancel aplicado.
- `TLC`: Si existe un tratado de libre comercio (1 = sí, 0 = no).
- `Frontera`: Si los países comparten frontera (1 = sí, 0 = no).
- `Relaciones`: Relaciones diplomáticas o políticas relevantes.
- `Religión`: Similaridad religiosa.
- `Colonia`: Relación colonial previa.

---

## 🚀 Modelos Implementados
LLM: Utilizamos el Large Language Model “deepseek-r1” de la herramienta de código abierto Ollama. Este modelo basado en Transformers está especializado en programación y razonamiento matemático. En nuestro proyecto deepseek-r1 tiene tres funciones claves:  interpretar lenguaje natural, generar código Python y formular análisis económico del resultado.

Librerias: utilizamos librerías tradicionales como pandas, numpy y matplotlib para el análisis y visualización del procesamiento del DataFrame, también se usó Gradio para la interfaz del  ChatBot.



---

## Resultados y Análisis
El ChatBot funciona correctamente: la interfaz se abre mediante Gradio, y el usuario puede ingresar preguntas en lenguaje natural de forma intuitiva. A través de la infraestructura construida, cada pregunta enviada es procesada por el modelo de lenguaje Deepseek-R1, el cual recibe instrucciones personalizadas (prompts) para entender el contexto de los datos y generar respuestas relevantes y estructuradas.

Al recibir la entrada del usuario, el modelo Interpreta la intención de la pregunta y procesa el contenido del DataFrame, usando la descripción estructurada que se le proporciona. Después procede a generar código Python específico que puede incluir operaciones estadísticas, transformación de datos y visualización, para lograr identificar automáticamente qué variables son más relevantes según el contexto de la pregunta.

El sistema luego ejecuta ese código y presenta al usuario un gráfico claro, con etiquetas, escalas logarítmicas cuando es necesario, y títulos informativos. Como también un análisis textual con predicciones, conclusiones o hallazgos económicos relevantes.

Este flujo permite que el ChatBot no solo entienda preguntas, sino que además tome decisiones analíticas:

•	Prioriza variables que tienen mayor correlación o impacto según el problema consultado.

•	Decide cuándo transformar escalas para mejorar la interpretación (por ejemplo, logaritmos en distribuciones sesgadas).

•	Presenta visualizaciones con estética y contenido adecuados para análisis económico.

La arquitectura del proyecto permite observar que el modelo razona paso a paso, lo cual se evidencia en cómo adapta el análisis según cada pregunta. El modelo también muestra su razonamiento explícito, aplicando criterios lógicos, económicos y estadísticos para seleccionar variables, formatos de gráficos y estructura del output.

El modelo también reconoce los factores económicos más importantes, ajusta los datos antes de graficar (por ejemplo, agrupamientos, escalas, filtrados) y genera predicciones o conclusiones cuando es pertinente. Esto demuestra que el sistema combina la potencia de los modelos LLM con un entorno de ejecución controlado, y que es capaz de realizar análisis empíricos completos sin intervención técnica del usuario.

---

## Conclusiones y Recomendaciones
El proyecto demuestra que es posible automatizar el análisis de datos económicos mediante la integración de modelos de lenguaje grandes con una interfaz accesible para el usuario. A través del uso del modelo Deepseek-R1, el sistema es capaz de interpretar preguntas en lenguaje natural, analizar un DataFrame económico y generar visualizaciones acompañadas de interpretaciones y predicciones relevantes. La incorporación de Gradio permite que la interacción con el modelo sea sencilla y efectiva, haciendo del ChatBot una herramienta valiosa tanto en entornos académicos como profesionales. Se observó que el modelo identifica variables clave según el contexto de la pregunta, aplica transformaciones cuando es necesario y genera resultados estructurados que facilitan la toma de decisiones o la presentación de hallazgos.

A partir de su funcionamiento, se recomienda al usuario seguir ciertas buenas prácticas para obtener mejores resultados del chatbot. En primer lugar, es importante formular preguntas claras, específicas y bien estructuradas, evitando ambigüedades que puedan confundir al modelo. En segundo lugar, se recomienda trabajar con un dataset bien organizado, con variables relevantes y sin inconsistencias, ya que la calidad de los datos influye directamente en la calidad del análisis generado. Por último, es aconsejable estar atento a posibles malentendidos en la interpretación de las preguntas por parte del modelo, revisando críticamente las respuestas y ajustando el input si es necesario para guiar mejor el análisis.

---

## 👥 Autores

Este proyecto fue desarrollado para IA Aplicada a la Economía – Período 2025-10.

Profesor: Juan Camilo Vega.

Institución: Universidad de los Andes.

Autores:

- Tomas Acevedo Echeverria - Autor principal
- Jennifer Paola Sarabia Solano - Autor principal
- Angela Michel Aparicio Sanabria - Autor principal
- Juan Jose Echavarria Villamizar - Autor principa
- Alejandro Alberto Gonzalez Londono - Autor principa

---

## 📦 Requisitos de Instalación

Para ejecutar este proyecto, asegúrate de tener instaladas las siguientes bibliotecas:

```bash
pip install 


