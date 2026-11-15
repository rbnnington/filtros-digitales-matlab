# Diseño e Implementación de Filtros Digitales en MATLAB

Este repositorio contiene el código y análisis de la práctica de **Señales y Sistemas (2026-3)** sobre el diseño de filtros digitales IIR y FIR en MATLAB para el procesamiento de señales contaminadas con ruido blanco.

## 📋 Descripción del Proyecto
Se generó una señal compuesta por tres componentes senoidales ($5\text{ Hz}$, $50\text{ Hz}$ y $250\text{ Hz}$) mezcladas con ruido blanco gaussiano ($f_s = 1000\text{ Hz}$). Se diseñaron tres filtros digitales para aislar cada frecuencia:
1. **Filtro IIR Pasa Bajos (Butterworth, orden 4):** Frecuencia de corte en $15\text{ Hz}$ para extraer la señal de $5\text{ Hz}$.
2. **Filtro FIR Pasa Bandas (Ventana Hamming, orden 100):** Banda de paso de $30\text{ Hz}$ a $80\text{ Hz}$ para extraer la señal de $50\text{ Hz}$.
3. **Filtro IIR Pasa Altos (Chebyshev Tipo I, orden 4):** Frecuencia de corte en $150\text{ Hz}$ para extraer la señal de $250\text{ Hz}$.

## 🛠️ Requisitos
* **MATLAB** (R2020a o superior) o **MATLAB Online**.
* **Signal Processing Toolbox** (necesaria para funciones como `butter`, `cheby1`, `fir1`, `freqz` y `filtfilt`).

## 🚀 Instrucciones de Ejecución
1. Clona este repositorio o descarga el archivo `filtros_digitales.m`.
2. Abre MATLAB y navega hasta la carpeta del proyecto.
3. Ejecuta el script escribiendo en la ventana de comandos:
```matlab
filtros_digitales
```
4. Se desplegarán dos ventanas con la respuesta en frecuencia de los filtros y la comparativa temporal/espectral de las señales.
