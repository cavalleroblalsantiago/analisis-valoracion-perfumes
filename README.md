# 🧪 Análisis de Valoración y Mercado de Perfumes (~24k Fragancias)

Un análisis de datos de extremo a extremo que explora qué factores determinan la calificación percibida de los perfumes en la comunidad de **Fragrantica** y si esa valoración se traduce en demanda de mercado.

---

## 📊 Descripción del Proyecto

El objetivo principal de este proyecto es responder a la pregunta de negocio:
> *Si una marca quisiera lanzar un perfume hoy, ¿qué características se asocian a una mejor valoración de la comunidad y cómo se comporta la demanda?*

Se analizó una base de datos enriquecida de aproximadamente **24.000 fragancias**, cubriendo variables como notas olfativas, acordes principales, perfumistas, marcas, país de origen, año de lanzamiento y métricas de interacción/votos.

---

## 🚀 Metodología y Etapas

1. **Auditoría y Limpieza de Datos:** 
   - Unificación de catálogos y tratamiento de valores nulos.
   - Detección de anomalías y sesgos (ej. ediciones limitadas/flankers con distorsiones en la varianza de votos).
2. **Ingeniería de Variables:**
   - Implementación de **suavizado bayesiano** (*Bayesian Average*) para la variable objetivo de valoración, evitando penalizar o inflar fragancias con muy pocos votos.
3. **Modelado Predictivo e Interpretabilidad:**
   - Entrenamiento con `HistGradientBoostingRegressor` y modelos de regresión lineal interpretable (`statsmodels`) para medir el peso relativo de notas, marcas y perfumistas.
4. **Análisis de Mercado:**
   - Evaluación de concentración de la demanda, segmentos y balance de oferta por acorde olfativo.

---

## 🛠️ Tecnologías Utilizadas

- **Lenguaje:** Python 3.10+
- **Análisis y Manipulación de Datos:** Pandas, NumPy
- **Machine Learning & Modelado:** Scikit-Learn, Statsmodels
- **Visualización:** Matplotlib, Seaborn

---

## 📦 Cómo Ejecutar este Proyecto

1. Clonar el repositorio:
   ```bash
   git clone [https://github.com/cavalleroblalsantiago/analisis-valoracion-perfumes.git](https://github.com/cavalleroblalsantiago/analisis-valoracion-perfumes.git)
   cd analisis-valoracion-perfumes
