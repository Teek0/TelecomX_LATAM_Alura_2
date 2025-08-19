# 📉 Predicción de Cancelación de Clientes (*Churn*) – TelecomX LATAM (Parte 2)

## 📝 Descripción
Este proyecto corresponde a la segunda fase del análisis de evasión de clientes (*Customer Churn*) en **TelecomX LATAM**.  
En esta etapa se construyeron y evaluaron **modelos predictivos de machine learning** para anticipar la cancelación de clientes, identificar los factores más influyentes y proponer estrategias de retención basadas en datos.  

El trabajo se realizó en **Google Colab**, lo que permite ejecutar todo el flujo de análisis y modelado sin necesidad de instalación local.

## 🎯 Objetivos
- Entrenar y comparar modelos de clasificación para predecir la cancelación de clientes.  
- Evaluar el desempeño con métricas estándar (Accuracy, Precision, Recall, F1-score y Matriz de Confusión).  
- Analizar la importancia de las variables en la decisión de cancelación.  
- Generar conclusiones y recomendaciones prácticas para el negocio.  

## 📂 Contenido del proyecto
- `2_TelecomX_LATAM.ipynb` → Notebook principal con:
  - Normalización y separación de datos.  
  - Análisis de correlación y dirigido.  
  - Entrenamiento de modelos: **Regresión Logística** (con normalización) y **Random Forest** (sin normalización).  
  - Evaluación de desempeño y comparación.  
  - Análisis de importancia de variables.  
  - Conclusiones y recomendaciones estratégicas.  
- `telecomx1_OHE.csv` → Dataset con variables preprocesadas mediante One Hot Encoding.  
- `instrucciones siguientes.md` → Guía de pasos para esta fase del proyecto.  

## 🚀 Ejecución en Google Colab
1. Subir el archivo `2_TelecomX_LATAM.ipynb` a tu Google Drive.  
2. Abrir el archivo con **Google Colaboratory**.  
3. Ejecutar las celdas en orden para reproducir el análisis y los resultados.  

## 📦 Dependencias
Google Colab incluye las principales librerías preinstaladas:  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  

No se requiere instalación adicional.  

## 📊 Resultados principales
- **Regresión Logística**: Accuracy ≈ 80%, con buen equilibrio entre precisión y recall, y sin señales de sobreajuste.  
- **Random Forest**: Accuracy ≈ 79%, pero con sobreajuste marcado (train ≈ 99.7%).  
- **Factores clave asociados a la cancelación**:
  - Contrato mensual.  
  - Baja antigüedad del cliente.  
  - Cargos mensuales elevados.  
  - Servicio de Fibra Óptica.  
  - Ausencia de servicios adicionales (seguridad, soporte, respaldo).  
- **Factores protectores**:
  - Contrato bienal.  
  - Antigüedad alta.  
  - Servicio DSL o planes básicos.  

## 🏆 Conclusiones
El modelo de **Regresión Logística** es el más recomendable en esta fase por su desempeño estable y su capacidad de interpretación.  
Los hallazgos permiten diseñar **estrategias de retención focalizadas**, tales como: incentivar contratos de largo plazo, programas de fidelización en clientes nuevos, y gestión diferenciada de clientes de alto gasto.
