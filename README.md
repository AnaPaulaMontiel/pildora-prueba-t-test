# 📊 Estructura de la Presentación: Prueba T de Student

Este repositorio contiene el material didáctico y visual correspondiente a la presentación sobre la **Prueba T de Student** dentro del módulo de Estadística Inferencial. A continuación, se detalla el orden, el hilo conductor y el contenido de las diapositivas que componen la exposición para facilitar la navegación del proyecto.

---

## 🗺️ Mapa de Contenido (Slide por Slide)

### 🔹 Bloque 1: Introducción y Fundamentos
* **Diapositiva 1: Portada**
  * **Contenido:** Título principal de la exposición.
  * **Enfoque:** Presentación de la Prueba T como herramienta fundamental para la comparación de medias y la validación de hipótesis en la investigación científica.
* **Diapositiva 2: Fundamentos del T-Test**
  * **Contenido:** Introducción al propósito central y la mecánica matemática detrás de la prueba.
* **Diapositiva 3: ¿Qué es la Prueba T?**
  * **Contenido:** Definición de la prueba estadística inferencial utilizada para determinar si existe una diferencia significativa entre las medias de dos grupos.
  * **Conceptos clave:** Evaluación de si la diferencia es real o producto del azar empleando el error estándar. [cite_start]Es ideal para muestras pequeñas ($n < 30$) o cuando la varianza poblacional es desconocida.
  * **Apoyo visual:** Gráfico de barras con puntuaciones de estudiantes (*Student Scores: Pre-test vs. Test*).

---

### 🔹 Bloque 2: Tipos de Prueba y Comportamiento Estadístico
* **Diapositiva 4: Tipos de Pruebas T**
  * **Muestras Independientes:** Comparación de las medias de dos grupos distintos y no relacionados (ej. comparar la presión arterial entre hombres y mujeres).
  * **Muestras Relacionadas (Pareadas):** Comparación de medias del mismo grupo en dos momentos diferentes (pre y post test) o pares emparejados.
* **Diapositiva 5: La Distribución T de Student**
  * **Contenido:** Explicación visual y teórica de la distribución T[cite: 44]. [cite_start]A diferencia de la distribución normal estándar ($Z$), la distribución T tiene "colas" más pesadas para reflejar la mayor incertidumbre al trabajar con muestras pequeñas.
  * **Apoyo visual:** Gráfico comparativo entre la curva de distribución normal (*Normal Dist.*) y la distribución T con grados de libertad específicos (*T-Dist., df=7*).

---

### 🔹 Bloque 3: Aplicación Práctica y Supuestos
* **Diapositiva 6: Supuestos del Modelo**
  * **Normalidad:** Se asume que los datos de ambos grupos siguen una distribución aproximadamente normal.
  * **Homocedasticidad:** Las varianzas de los grupos deben ser similares, evaluado mediante la Prueba de Levene.
  ***Independencia:** Las observaciones dentro y entre los grupos deben ser independientes entre sí.
* **Diapositiva 7: Ejemplo de Visualización**
  * **Contenido:** Caso práctico con datos numéricos para ilustrar el contraste.
  * **Planteamiento:** Comparativa entre un *Grupo Control* (65 pts) y un *Grupo Experimental* (82 pts) para plantear la incógnita: ¿Es esta diferencia de 17 puntos estadísticamente significativa o fruto del error de muestreo?

---

### 🔹 Bloque 4: Toma de Decisiones y Análisis Crítico
* **Diapositiva 8: Decisión de la Prueba (Matriz)**
  * **Contenido:** Tabla de decisiones para seleccionar la prueba estadística correcta según el escenario y sus supuestos clave:
    
    | Escenario | Prueba Sugerida | Supuesto Clave |
    | :--- | :--- | :--- |
    | Muestras independientes con varianzas iguales | T de Student Clásica | Normalidad y Homocedasticidad |
    | Muestras independientes con varianzas desiguales | Prueba T de Welch | No requiere varianzas iguales |
    | Mismo sujeto medido dos veces | T de Muestras Pareadas | Diferencia normal entre medidas |

* **Diapositiva 9: El Criterio de Decisión**
  * **Contenido:** Uso del nivel de significancia estándar ($\alpha = 0.05$) e interpretación del p-valor.
  * **Regla de oro:** Si el $p\text{-valor} < 0.05$, se rechaza la hipótesis nula ($H_0$), lo que implica que hay menos de un 5% de probabilidad de que la diferencia sea debida al azar (diferencia significativa)
* **Diapositiva 10: Importancia del Resultado**
  * **Contenido:** Contraste entre *Significancia estadística vs. Magnitud del efecto*
  * **Concepto clave:** Un p-valor bajo indica que el efecto existe, pero no qué tan grande es[cite: 87]. [cite_start]Se introduce la **D de Cohen** para medir la magnitud real y dar contexto práctico o clínico al hallazgo.
* **Diapositiva 11: Consideraciones Críticas**
  * **Outliers:** Los valores atípicos pueden distorsionar la media y aumentar el error estándar, invalidando el test.
  * **Tamaño de Muestra:** Con muestras muy grandes, incluso diferencias minúsculas pueden resultar "significativas" artificialmente.
  * **Alternativas No Paramétricas:** Uso de la prueba de **Mann-Whitney U** si no se cumple el supuesto de normalidad.
  * **P-hacking:** Importancia de evitar realizar múltiples comparaciones sin los ajustes adecuados como la corrección de Bonferroni.

---

## 🛠️ Herramientas y Formato
* **Diseño de Diapositivas:** Google Slides (Presentaciones de Google).
* **Documentación matemática:** Formato Markdown compatible con expresiones en bloque e inline mediante expresiones matemáticas estándar.
* Elaborado por Ana Paula Montiel
