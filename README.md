# TelecomX_LATAM-Challenge
Challenge Telecom X: análisis de evasión de clientes

# 📊 Análisis de Churn para TelecomX

## 1. Visión General del Proyecto
Este proyecto se centra en un análisis exhaustivo de los datos de clientes de TelecomX con el objetivo de identificar los factores clave que contribuyen a la evasión de clientes (churn). El informe resultante busca proporcionar una comprensión clara de los segmentos de clientes en riesgo y ofrecer recomendaciones estratégicas para mejorar la retención.

## 2. Metodología
### Tecnologías y Librerías Utilizadas
* `pandas`: Manipulación y análisis de datos.
* `numpy`: Soporte para arrays y operaciones numéricas.
* `matplotlib.pyplot` y `seaborn`: Creación de visualizaciones para el análisis exploratorio.

### 2.1. Extracción y Carga de Datos
* Los datos se cargaron directamente desde un archivo JSON alojado en un repositorio de GitHub.

### 2.2. Preprocesamiento de Datos
* **Aplanamiento de la estructura:** Se normalizó la estructura anidada del archivo JSON para crear un DataFrame plano y tabular.
* **Limpieza y transformación:** Se revisó la integridad de los datos para asegurar que no hubiera valores nulos ni duplicados.
* **Ajuste de tipos de datos:** Se corrigieron los tipos de datos en columnas numéricas y se transformaron variables categóricas (como `Partner` y `InternetService`) en un formato binario (1 y 0) para su posterior análisis.

## 3. Principales Hallazgos del Análisis
El análisis exploratorio reveló insights cruciales sobre el comportamiento de los clientes:
* **Tasa de Churn General:** TelecomX enfrenta una tasa de churn del **27%**.
* **Perfil de Mayor Riesgo:** La combinación de clientes con un **contrato de mes a mes** y servicio de **Fibra Óptica** representa el segmento más propenso a la cancelación.
* **Antigüedad y Costo:**
    * Los clientes que cancelan tienen una antigüedad significativamente menor, con una mediana de **10 meses**, en comparación con la mediana de **40 meses** de los clientes leales.
    * Además, los clientes que abandonan el servicio suelen tener **cargos mensuales más altos**.

## 4. Conclusiones y Recomendaciones Estratégicas
**Conclusión principal:** El churn está fuertemente influenciado por clientes nuevos con planes flexibles y servicios de alto costo, lo que sugiere una posible falta de percepción de valor.

**Recomendaciones:**
1.  **Focalizar la Retención:** Crear ofertas especiales o descuentos dirigidos a los clientes del segmento de "Fibra Óptica + Contrato Mensual" para incentivarlos a migrar a planes de mayor duración.
2.  **Mejorar la Experiencia Inicial:** Reforzar el proceso de onboarding durante los primeros tres meses para construir lealtad y demostrar el valor del servicio desde el principio.
3.  **Evaluar la Oferta de Fibra Óptica:** Realizar una revisión de la estructura de precios y la calidad del servicio de fibra para asegurar su competitividad y que cumpla con las expectativas de los clientes que pagan más.
