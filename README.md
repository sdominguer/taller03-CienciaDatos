# Análisis de Series de Tiempo y Conectómica: Agro-Intelligence

Este proyecto implementa un ecosistema de análisis avanzado para series de tiempo con ruido sistémico, utilizando modelos auto-regresivos, pruebas de causalidad de Granger y análisis de topología de redes para identificar dependencias críticas entre activos.

## Descripción del Proyecto
El flujo de trabajo aborda la problemática de los datos ruidosos en entornos agrícolas/financieros, permitiendo filtrar la señal del ruido, modelar la dependencia temporal y visualizar la red de influencias mediante grafos dirigidos.

### Componentes Principales:
1.  **Ingesta y Limpieza:** Carga de datos geoespaciales y temporales (`agro_noise.csv`).
2.  **Análisis Estadístico:** Evaluación de estacionariedad mediante el test de **Augmented Dickey-Fuller (ADF)**.
3.  **Modelado Predictivo:** Ajuste de modelos **AR (AutoReg)** y **ARMA (3,1)** para la reconstrucción de señales.
4.  **Simulación de SNR:** Evaluación del impacto del ruido en la fidelidad de los datos (Señal vs. Ruido).
5.  **Análisis de Redes (Topología):** Construcción de matrices de adyacencia basadas en correlaciones de Pearson y visualización de grafos.
6.  **Causalidad de Granger:** Identificación de relaciones causa-efecto no simétricas entre múltiples series.

## Requisitos
Para ejecutar este notebook en Google Colab o de forma local, necesitas las siguientes librerías:

```python
pip install numpy pandas matplotlib seaborn statsmodels networkx scikit-learn
