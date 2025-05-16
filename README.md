# TradeBot: Inteligencia Comercial Interactiva

## 📌 Descripción del Proyecto

Este proyecto aplica técnicas de **procesamiento de lenguaje natural (NLP)** y **modelos generativos** al análisis económico, específicamente al estudio del comercio internacional utilizando el modelo de gravedad. Se desarrolla un asistente económico capaz de interpretar consultas sobre exportaciones, distancias, PIB, acuerdos comerciales, entre otros factores, integrando componentes de machine learning, análisis de datos y retrieval-augmented generation (RAG).

---

## 🎯 Objetivo del Proyecto

Desarrollar una solución basada en IA que permita analizar, predecir y explicar dinámicas del comercio bilateral entre países utilizando datos reales y modelos generativos. El sistema debe responder preguntas del usuario, hacer análisis de datos y generar predicciones usando una interfaz amigable.

---

## 📊 Descripción del Dataset

🔗 **Fuente** :  Clase comercio internacional, Universidad de los Andes


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
### ✅ Funcionamiento del ChatBot – Resumen en Bullet Points

- La interfaz se abre correctamente mediante **Gradio**, permitiendo que el usuario ingrese preguntas en lenguaje natural de forma intuitiva.
- Cada pregunta es procesada por el modelo **Deepseek-R1**, el cual recibe **prompts personalizados** para entender el contexto de los datos y generar respuestas relevantes.
- El modelo:
  - Interpreta la intención de la pregunta.
  - Procesa el contenido del DataFrame usando su descripción estructurada.
  - Genera código Python específico con operaciones estadísticas, transformación de datos o visualización.
- El sistema **ejecuta automáticamente** ese código y entrega:
  - Un **gráfico claro**, con etiquetas, escalas logarítmicas (cuando se requieren) y títulos informativos.
  - Un **análisis textual** con predicciones, conclusiones o hallazgos económicos.

---

### 🔍 Capacidades analíticas del sistema

- Prioriza variables con **mayor correlación o impacto** según el problema consultado.
- Decide cuándo aplicar **transformaciones de escala** para mejorar la interpretación (por ejemplo, logaritmos).
- Presenta **visualizaciones limpias y útiles** para el análisis económico.

---

### 🧠 Razonamiento paso a paso del modelo

- El modelo **razona paso a paso**, adaptando cada análisis al contenido y contexto de la pregunta.
- Aplica criterios **lógicos, económicos y estadísticos** para seleccionar variables, formatos de visualización y estructura del resultado.
- Reconoce los factores económicos relevantes y ajusta los datos antes de graficar (agrupamientos, filtrado, escalado).

---

### 🧩 Conclusión

- El sistema combina la potencia de los **modelos LLM** con un entorno de ejecución controlado.
- Permite realizar **análisis empíricos completos sin intervención técnica** del usuario.


---

## Conclusiones y Recomendaciones
### ✅ Conclusiones del Proyecto

- El proyecto demuestra que es posible **automatizar el análisis de datos económicos** mediante la integración de modelos de lenguaje grandes con una interfaz accesible para el usuario.
- A través del uso del modelo **Deepseek-R1**, el sistema interpreta preguntas en lenguaje natural, analiza un DataFrame económico y genera visualizaciones acompañadas de interpretaciones y predicciones relevantes.
- La incorporación de **Gradio** facilita la interacción con el modelo, haciendo del chatbot una herramienta útil en entornos **académicos y profesionales**.
- El modelo identifica variables clave según el contexto, aplica transformaciones cuando es necesario y genera resultados estructurados que **facilitan la toma de decisiones** o la presentación de hallazgos.

---

### 🧭 Recomendaciones de uso

- Formular **preguntas claras y específicas**, evitando ambigüedades que puedan confundir al modelo.
- Usar un **dataset limpio y bien estructurado**, con variables relevantes y sin inconsistencias.
- Revisar críticamente las respuestas, ya que pueden surgir **malentendidos en la interpretación del input** por parte del modelo. Ajustar la formulación si es necesario para guiar mejor el análisis.

---

### ⚠️ Limitaciones del sistema

- El modelo depende del contenido y estructura del DataFrame. Si los datos están incompletos o mal etiquetados, el análisis será poco fiable.
- No hay verificación automática de si los resultados tienen sentido económico; el modelo puede hacer supuestos implícitos erróneos.
- Las transformaciones aplicadas (como escalas logarítmicas o agrupamientos) no siempre son las óptimas sin contexto humano adicional.
- Si bien se simula razonamiento paso a paso, el modelo no “razona” en sentido humano: **las respuestas son estadísticas, no lógicas.**
- Puede fallar al manejar preguntas complejas, mal redactadas o fuera del dominio del dataset proporcionado.



---

## 👥 Autores

Este proyecto fue desarrollado para IA Aplicada a la Economía – Período 2025-10.

Profesor: Juan Camilo Vega.

Institución: Universidad de los Andes.

Autores:

- Tomás Acevedo Echeverria - Autor principal
- Jennifer Paola Sarabia Solano - Autor principal
- Angela Michel Aparicio Sanabria - Autor principal
- Juan Jose Echavarria Villamizar - Autor principal
- Alejandro Alberto Gonzalez Londono - Autor principal

---


