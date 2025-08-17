# Challenge_Telecom_X_2 Predicción de Cancelación de Clientes (churn)

**📊 Descripción del Proyecto**

  Este proyecto es la segunda parte del desafío de abandono clientes, tiene como objetivo analizar los datos de clientes de Telecom X para identificar los factores que influyen en la cancelación del servicio        (churn) y desarrollar modelos predictivos para predecir qué clientes tienen una alta probabilidad de cancelar. El análisis y los modelos resultantes buscan proporcionar información estratégica para implementar    acciones de retención de clientes.

**📂Contenido del Repositorio**

•	df_telecomx2.csv: Archivo de datos utilizado para el análisis.

•	notebook.ipynb: El cuaderno de Jupyter/Colab que contiene todo el código de análisis, preprocesamiento, modelado y evaluación.

•	README.md: Este archivo.

**🛠️ Configuración del Entorno**

  Para ejecutar el notebook, necesitas tener instaladas las siguientes librerías de Python:
  
•	pandas

•	numpy

•	seaborn

•	matplotlib

•	scikit-learn

•	imbalanced-learn

•	xgboost

•	statsmodels

Puedes instalarlas usando pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn imbalanced-learn xgboost statsmodels 
```

**🔍 Análisis de Datos y Metodología**

  El proyecto sigue los siguientes pasos:

1.	Carga y Exploración de Datos: Los datos de df_telecomx2.csv fueron cargados y se realizó un análisis exploratorio para entender la distribución de las variables y la proporción de clientes que cancelan. Se        identificó un desbalance significativo en la clase objetivo.
	
2.	Preprocesamiento de Datos: Se eliminaron columnas irrelevantes. Las variables categóricas fueron codificadas utilizando One-Hot Encoding.
	
3.	Modelado: Se entrenaron y evaluaron varios modelos de clasificación para predecir la cancelación de clientes, incluyendo:
   
	  o	Árbol de Decisión

    o	KNN (K-Nearest Neighbors)
  	
    o	Random Forest
  	
    o	Regresión Logística
  	
    o	SVM (Support Vector Machine)
  	
    o	XGBoost Se utilizó SMOTE para balancear los datos de entrenamiento y abordar el desbalance de clases.
  	
  	
4.	Evaluación de Modelos: Los modelos fueron evaluados utilizando métricas como Exactitud (Accuracy), Precisión (Precision), Sensibilidad (Recall) y F1-Score, así como curvas ROC y AUC.
	
5.	Selección del Modelo Champion: Se seleccionó la Regresión Logística con SMOTE como el modelo "champion" basándose en un equilibrio entre Precisión y Sensibilidad.
	

**🔄 Resultados**

  El modelo de Regresión Logística fue elegido como el mejor, demostró ser el más adecuado para este problema, logrando un buen balance en la identificación de clientes que cancelan.

**📋Interpretación del Modelo y Factores Clave**

  El análisis de importancia de variables de los modelos (Regresión Logística, SVM, XGBoost y Random Forest) reveló que los factores más influyentes en la cancelación de clientes son:

•	Duración del servicio (Tiempo de cliente): Los clientes con menor antigüedad son más propensos a cancelar.

•	Soporte técnico / atención al cliente: La calidad del soporte es crucial para la retención.

•	Facturación electrónica / cargos adicionales: La transparencia y claridad en la facturación es importante.

•	Uso de servicios adicionales: Los clientes que utilizan más servicios adicionales tienden a permanecer.



**📌 Conclusiones y Recomendaciones Estratégicas**

  Basado en los hallazgos, se proponen las siguientes recomendaciones para reducir la tasa de cancelación:

•	Fidelización temprana: Implementar estrategias de retención en los primeros meses de servicio.

•	Mejora continua del soporte al cliente: Asegurar una resolución eficiente de problemas y una atención de calidad.

•	Transparencia en la facturación: Comunicar claramente los costos y beneficios.

•	Promover Contratos a Largo Plazo: Implementar incentivos atractivos (descuentos, beneficios adicionales) para alentar a los clientes con contratos mes a mes a cambiar a planes de uno o dos años.

•	Destacar el Valor de los Servicios Adicionales: Promocionar activamente los beneficios de la seguridad en línea y el soporte técnico, quizás ofreciendo pruebas gratuitas o paquetes combinados para aumentar la     adopción y, potencialmente, la lealtad del cliente.

•	Fomentar la Agrupación de Servicios: Resaltar las ventajas de tener múltiples servicios (como teléfono e internet) con la empresa para aumentar la dependencia y reducir la propensión a cambia

•	Análisis de Segmentación de Clientes: Realizar análisis de segmentación de clientes para entender si diferentes grupos de clientes tienen diferentes impulsores 
  de cancelación y si se necesitan modelos o estrategias de retención específicas para cada segmento.
  
•	Análisis de Costo-Beneficio: Evaluar el costo de implementar diferentes estrategias de retención en comparación con el valor de los clientes retenidos para optimizar la inversión en retención.

  Estas estrategias, respaldadas por el análisis de datos y el modelo predictivo, pueden ayudar a Telecom X a mejorar la retención de sus clientes.

  

**👥 Autor**

**Cristina Valenzuela**

**Curso: Formación en Data Science**

**Programa ONE Alura Latam**
  
