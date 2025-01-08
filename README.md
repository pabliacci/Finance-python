# Clustering de Tickers del IPSA

Este proyecto utiliza técnicas de clustering para analizar y agrupar los tickers de las empresas que componen el índice IPSA (Índice de Precios Selectivo de Acciones). 

## Objetivo
El objetivo principal es identificar patrones y similitudes entre las empresas del IPSA, basándonos en características financieras o de mercado, con el fin de generar insights útiles para análisis financieros y de inversión.

## Preview
- **results/**: Gráficos, modelos y otros resultados generados por el análisis.
![Cluster_IPSA_kmeans](https://github.com/user-attachments/assets/cb356b44-52a7-410a-8760-b3f1223eac53)

## Tecnologías Utilizadas
- **Python**: Lenguaje principal.
- **Librerías**: 
  - `pandas` y `numpy` para manejo y análisis de datos.
  - `scikit-learn` para algoritmos de clustering.
  - `matplotlib` y `seaborn` para visualización.
- **Jupyter Notebook**: Para documentar y presentar el análisis.

## Cómo Usar
1. Clona este repositorio:
   ```bash
   git clone https://github.com/pabliacci/Finance-python.git

# Análisis de VaR en los Tickers del IPSA

Este proyecto tiene como objetivo calcular y analizar el Valor en Riesgo (VaR) para los principales tickers del índice IPSA, clasificándolos en dos grupos: los 5 tickers con mayor volumen de transacciones y los 5 con menor volumen. Utilizamos diferentes metodologías para el cálculo del VaR, lo que nos permitió observar cómo las características de los activos afectan el riesgo estimado.

## Preview

![preview_VaR](https://github.com/user-attachments/assets/a727e331-ec98-48ad-9781-64404f977109)


## Metodología

Se utilizaron las siguientes metodologías para calcular el VaR con un nivel de confianza del 95%:

1. **VaR Histórico:** Basado en los rendimientos históricos.
2. **VaR por Varianza-Covarianza:** Supone una distribución normal de los rendimientos.
3. **VaR por Simulación de Monte Carlo:** Genera escenarios simulados para los precios futuros.
4. **VaR Cornish-Fisher:** Ajusta la distribución para capturar eventos extremos.

Adicionalmente, se calcularon medidas complementarias como la desviación estándar y la semidesviación para evaluar la volatilidad y los riesgos a la baja.

## Datos

Los datos utilizados en este análisis provienen de precios históricos de los tickers del IPSA, junto con información sobre el volumen de transacciones. Los tickers fueron clasificados en dos grupos:

- **5 tickers con mayor volumen de transacciones:** Activos altamente negociados.
- **5 tickers con menor volumen de transacciones:** Activos con menor liquidez.

## Descubrimientos

1. **Volatilidad:** Los tickers con mayor volumen tienden a tener mayor semidesviación, lo que indica un mayor riesgo a la baja.
2. **VaR:** Los tickers menos negociados presentan VaR más altos en metodologías que capturan eventos extremos, como Monte Carlo y Cornish-Fisher.
3. **Comparación de métodos:** La metodología Cornish-Fisher demuestra ser más sensible a colas gruesas en la distribución de rendimientos, ajustándose mejor a eventos atípicos.

## Repositorio

Este repositorio incluye:

- Código para la implementación de cada metodología de cálculo de VaR.
- Gráficos que ilustran la distribución de rendimientos y los valores de VaR.
- Documentación sobre las herramientas y bibliotecas utilizadas.

## Herramientas Utilizadas

- Python (Pandas, NumPy, SciPy, Matplotlib, Seaborn)
- Jupyter Notebook para análisis interactivo

## Conclusión

Este análisis destaca cómo el volumen de transacciones y la volatilidad afectan las estimaciones de riesgo en los activos del IPSA. Los resultados pueden ser utilizados por analistas financieros y gestores de portafolio para tomar decisiones informadas sobre la gestión de riesgos.

## Contacto

Si tienes preguntas o comentarios sobre este proyecto, no dudes en contactar a [Pablo Gonzalez](mailto:pabloagonz@fen.uchile.cl) o abrir un issue en este repositorio.

