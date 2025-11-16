# K-Means-Clustering

📘 Customer Segmentation Using K-Means (RFM Model)

Proyecto académico – Inteligencia Artificial
Universidad de Las Américas (UDLA)

👥 Integrantes

Jair Rueda

Andrei Flores

Wanderley Flores

Matías Romo

Andre Mateo Rosero

🎯 Descripción del Proyecto

Este proyecto implementa una segmentación de clientes basada en las métricas RFM (Recency, Frequency, Monetary) utilizando el dataset Online Retail del repositorio UCI Machine Learning.

Se realiza:

Limpieza del dataset

Cálculo de métricas RFM por cliente

Normalización con StandardScaler

Selección óptima de clusters usando Elbow Method y Silhouette Score

Entrenamiento del modelo K-Means con k = 4

Análisis detallado de los 4 segmentos de clientes

Visualizaciones (Heatmap, Scatterplot, PCA, t-SNE)

Comparación con Clustering Jerárquico

Evaluación de estabilidad mediante Adjusted Rand Index (ARI)

El objetivo es identificar grupos de clientes con comportamientos similares para apoyar decisiones de marketing, retención y estrategias comerciales.

📂 Estructura del Repositorio
📁 data
   └── Online Retail.xlsx          # Dataset original utilizado
📄 JAMWR.ipynb                      # Notebook principal con todo el análisis
📄 JAMWR.html                       # Notebook exportado a HTML
📄 README.md                        # Este archivo

🧠 Tecnologías y Librerías Principales

Python 3.12

pandas, numpy

matplotlib, seaborn

scikit-learn (KMeans, StandardScaler, Silhouette, ARI, t-SNE, PCA)

nbconvert (exportación a HTML)

🚀 Cómo ejecutar el Notebook
1️⃣ Clona o descarga el repositorio
git clone (https://github.com/MateoRosero/K-Means-Clustering)

2️⃣ Abre el notebook

En Jupyter, Google Colab o VSCode:

JAMWR.ipynb

3️⃣ Asegúrate de que el dataset esté ubicado en:
/data/Online Retail.xlsx


Si usas Google Colab, cambia la ruta a:

df = pd.read_excel('/content/data/Online Retail.xlsx')

📊 Resumen de Resultados
🔹 Mejor valor de k:

k = 4, según:

Método del Codo

Silhouette Score (máximo entre k=4 y k=5)

🔹 Interpretación de Clusters

Cluster 2 – VIP / Alto Valor
Compran mucho, con alta frecuencia y gastan más que todos.

Cluster 3 – Frecuentes Nivel Medio
Compran seguido y gastan una cantidad considerable.

Cluster 0 – Clientes Promedio
Recencia y frecuencia media.

Cluster 1 – Clientes Inactivos
Mucho tiempo sin comprar, baja frecuencia y bajo gasto.

🧪 Bonus

✔ Clustering Jerárquico (Agglomerative)

K-Means obtiene mejor Silhouette Score y clusters más compactos.

✔ Estabilidad con ARI

El modelo logró un ARI ≈ 0.87, mostrando alta consistencia entre ejecuciones.

✔ t-SNE Visualization

Confirma separación clara de los grupos, especialmente el cluster VIP.

🏁 Conclusión General

K-Means aplicado sobre métricas RFM permite identificar segmentos de clientes bien definidos, estables y accionables.
Los análisis complementarios (PCA, t-SNE, Jerárquico, ARI) confirman la calidad del modelo y su utilidad para diseñar campañas de marketing personalizadas, optimizar recursos y mejorar la retención.
