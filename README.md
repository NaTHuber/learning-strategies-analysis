# Estrategias de aprendizaje y su relación con el rendimiento académico

Este proyecto analiza cómo diferentes estrategias de aprendizaje (autogestión, motivación, técnicas de estudio) se relacionan con el rendimiento académico percibido en estudiantes universitarios. A través de un análisis estadístico y un modelo de regresión lineal, se identifican los predictores más relevantes que influyen en dicha percepción.

---

## Objetivo

Explorar la relación entre distintos factores psicológicos de aprendizaje y el rendimiento académico percibido, con el fin de responder a dos preguntas guía:

- ¿Qué variables tienen mayor correlación con el rendimiento académico?
- ¿Cuáles son los predictores más fuertes de buen desempeño académico?

---

## Dataset

**Nombre**: Learning Strategies in Higher Education  
**Fuente**: [Mendeley Data (Carlos Ramos-Galarza et al., 2025)](https://data.mendeley.com/datasets/7vgyndhb87/5)  
**Ubicación**: Chile y Ecuador  
**Dimensiones evaluadas**:
- Percepción del rendimiento académico
- Autogestión del aprendizaje
- Estrategias de motivación consciente
- Técnicas de aprendizaje profundo

---

## Análisis

### Exploración de datos
- Limpieza de columnas, renombramiento de ítems del cuestionario (GAEU-1).
- Agrupación de ítems por factor psicológico (autogestión, motivación, etc.).
- Visualización de correlaciones entre factores.

### Resultados clave

- La **autogestión del aprendizaje es el factor que más influye en la percepción de rendimiento académico de los estudiantes**, con un coeficiente de 0.427. Esto se refuerza con el resultado obtenido de 0.59 en la sección de correlaciones. 
- La **motivación consciente** y las **técnicas de aprendizaje profundo** también mostraron correlaciones positivas, aunque más débiles.
- El modelo explica cerca del 39% de la variabilidad del rendimiento percibido (R² = 0.391), lo cual se puede considerarse significativo en estudios de percepción y autoevaluación.

Este hallazgo sugiere que **intervenir en estrategias de autogestión puede tener un mayor impacto en la percepción de éxito académico que enfocarse solamente en la motivación o en técnicas aisladas de estudio.**

### Modelo de regresión lineal múltiple

```python
Rendimiento_percibido =
    1.08
  + 0.427 * Autogestión
  + 0.193 * Motivación
  + 0.068 * Técnicas de estudio
```

## Tecnologías usadas

- Python (pandas, seaborn, matplotlib, scikit-learn)

- Jupyter Notebooks

- Markdown y LaTeX (para documentación)

## Ideas para el futuro 
- Análisis por subgrupos: explorar diferencias por país, género, edad o universidad para detectar patrones más específicos.

- Visualizaciones interactivas: desarrollar un mini-dashboard con Streamlit para navegar dinámicamente entre factores y resultados.

- Ampliación del modelo: probar modelos no lineales (Random Forest, XGBoost).

- Validación cruzada: dividir los datos en train/test o aplicar K-Fold CV para evaluar la robustez del modelo.

## Contacto 
Si te interesó el proyecto puedes escribirme al email: [nbaezhuber@gmail.com](mailto:nbaezhuber@gmail.com)