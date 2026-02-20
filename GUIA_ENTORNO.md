# 🛠️ Guía de Configuración del Entorno: CORE-PROJECT

Esta guía detalla cómo conectar las tres herramientas principales de nuestro ecosistema para el caso **easyMoney**. [cite_start]Es fundamental seguir estos pasos para asegurar la colaboración sobre código ajeno y la integridad de los datos[cite: 10].

## 1. Conexión Google Colab ↔️ Google Cloud Storage (GCS)
[cite_start]Dado que los datos residen en un bucket y no en local, debemos autenticarnos en cada sesión de trabajo para leer las 17 particiones de histórico[cite: 77, 78].

Ejecuta este bloque en la primera celda de tu notebook:

```python
from google.colab import auth
import pandas as pd

# Autenticación de tu cuenta de Google
auth.authenticate_user()

# Configuración del acceso al Bucket
BUCKET_NAME = "coreproyecto-ds-datos"
RAW_DATA_PATH = f"gs://{BUCKET_NAME}/raw/"

print("✅ Conectado exitosamente al almacenamiento de easyMoney")
