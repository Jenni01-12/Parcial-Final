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

---

## Conclusiones y Recomendaciones


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


