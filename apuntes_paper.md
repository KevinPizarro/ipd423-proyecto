#### Objetivo: 
Usar la metodología espacio-temporal de wavelets-chaos para el analisis de EEG en las bandas de frecuencia delta, theta, alpha y beta para descubrir potenciales patrones de anormalidad para Alzheimer.

#### Experimento:
8 segundos de segmentos de EEG (19 canales) para gente con AD y gente sin AD, con ojos abiertos y con ojos cerrados. Edad promedio 71. Sampling rate del EEG = 128 Hz. 1096 EEGs

#### Problema:
No existe un test *in vivo* para el diagnóstico de AD. Es un desorden neurodegenerativo muy común, cerca de 5 millones de personas en USA. ***(2008 ver avance hasta 2022)***

#### Solución:
Caracterizar el cerebro desde unas perspectiva no-lineal, caótica y dinámica. Por ello se utilizan analisis por sub bandas, técnicas como CD y Lyapunov.

Nuestro ground-truth es el criterio de diagnóstico NINCDS-ADRDA and DSM-III-R 

Uso de análisis mediante wavelets. Descomposición usando transformada wavelets de Daubechies de 4to orden. Luego reconstruimos con la transformada de wavelets inversa -> recuperando las 4 sub-bandas de respuesta fisiológica.
	Nos entrega CD y LLE para cada sub-banda y el EEG general.

Cálculos estadísticos se realizan mediante el test ANOVA.

---

#### GLOSARIO

- CD: Correlation Dimension. Se potencia en tareas cognitivas o cuando el cerebro está "despierto". REpresenta la complejidad.
- LLE Largest lyapunov Exponent.Representa qué tan caótico es.
- AD: Alzheimer Disease.
- EEG slowing:
- Reduced coherence:


#### Preguntas
One-way ANOVA? Three-way factorial ANOVA?