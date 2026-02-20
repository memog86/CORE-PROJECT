# 📂 Documentación Técnica: El Caso easyMoney

Este documento contiene las especificaciones técnicas proporcionadas por el departamento de IT (Frank) para el desarrollo del proyecto final.

## 🛠️ Acceso y Origen de los Datos
Debido a políticas de seguridad y para no comprometer el ERP de la compañía, no trabajaremos directamente sobre la base de datos de producción.

* **Fuente de datos:** Volcado de la base de datos modelada para el autoservicio de BI con ReportServer.
* **Ubicación:** Los archivos residen en la carpeta `data` (en nuestro caso, el bucket `gs://coreproyecto-ds-datos/raw/`).
* **Temporalidad:** Solo disponemos de **17 particiones de histórico**.
* **Limitaciones:** La información anterior a estas particiones se encuentra en un backup inalcanzable, ya que no era un requisito del proyecto original modelizarla.

## 📊 Estructura del Dataset
* **Detalle de campos:** Se ha adjuntado un archivo `.txt` con la descripción de cada columna del dataset.
* **Foco del análisis:** El área comercial (Carol) requiere centrar el análisis solo en los datos que aporten valor a las ventas, no en la totalidad de la base disponible.

## 💻 Herramientas Autorizadas
Siguiendo las instrucciones de IT y los requerimientos de la Tarea 1:
1.  **Python:** Obligatorio para realizar el *Data Cleaning* y la construcción de las tablas del modelo de datos.
2.  **Power BI:** Recientemente adquirido por la empresa. Se utilizará para la construcción de los dashboards de seguimiento de KPIs y análisis *Deep Dive*.

## ⚠️ Notas de Integración
* El traspaso de la función de *Analytics* desde IT hacia el equipo de Marketing es una decisión estratégica de la CEO (Carol).
* Es vital asegurar que el código sea comprensible para todos, ya que el trabajo en equipo y la colaboración sobre código
