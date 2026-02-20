# 🚀 CORE-PROJECT: Estrategia Data-Driven para easyMoney

Este repositorio contiene el proyecto final del Máster de Data Science, enfocado en transformar la comercializadora financiera **easyMoney** en una compañía orientada a datos. El objetivo principal es maximizar la rentabilidad de la cartera actual de clientes mediante analítica avanzada y marketing predictivo.

## 🏦 Contexto de Negocio
Tras 4 años de fuerte captación, easyMoney necesita alcanzar la rentabilidad exigida por sus inversores (Lion Global Management). El proyecto se centra en reorientar la estrategia desde la captación masiva hacia el aumento de la penetración de productos en la base de clientes actual, siguiendo la estrategia de penetración de mercado de la matriz de Ansoff.

[Image of Ansoff Matrix showing Market Penetration strategy]

## ☁️ Infraestructura y Datos
Para este proyecto, el equipo utiliza una arquitectura híbrida que garantiza seguridad y escalabilidad:

* **Almacenamiento de Datos:** Google Cloud Storage.
    * **Bucket Principal:** `gs://coreproyecto-ds-datos`.
    * **Directorio /raw**: Datos inmutables con 17 particiones de histórico.
    * **Directorio /processed**: Datasets limpios y transformados en Python listos para el modelo de datos.
* **Entorno de Ejecución:** Google Colab para procesamiento y modelado en Python.
* **Visualización:** Power BI para el desarrollo de Dashboards estratégicos de ventas.

## 🛠️ Roadmap del Proyecto
El trabajo se divide en cuatro tareas críticas definidas por la dirección:

1.  **Análisis de Ventas & Dashboards (Tarea 1):** Limpieza de datos con Python y creación de KPIs en Power BI para el Comité de Dirección.
2.  **Modelo de Propensión (Tarea 2):** Desarrollo de modelos predictivos para identificar clientes propensos a la compra de productos financieros.
3.  **Segmentación de Clientes (Tarea 3):** Identificación de 7 u 8 grupos de clientes similares para orientar la actividad comercial.
4.  **Caso de Uso & ROI (Tarea 4):** Estimación del retorno económico de una campaña específica basada en las propensiones y segmentos obtenidos.

[Image of Data Science project lifecycle from data cleaning to model deployment]

## 📂 Estructura del Repositorio
```text
CORE-PROJECT/
├── notebooks/   # Desarrollo de modelos y limpieza (Python)
├── src/         # Funciones modulares y scripts de soporte (.py)
├── docs/        # Diccionario de datos y requerimientos de negocio
├── .gitignore   # Archivo de exclusión de datos pesados
└── README.md    # Documentación principal del proyecto
