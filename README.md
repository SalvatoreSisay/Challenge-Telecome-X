# Challenge Telecom X 📱

## 🎯 Bienvenida

Bienvenido al **Challenge Telecom X**, un proyecto dedicado al análisis exploratorio de datos y procesamiento ETL sobre la **evasión de clientes** en la empresa Telecom X.

## 📊 Descripción del Desafío

Telecom X enfrenta una **alta tasa de cancelaciones** y necesita comprender los factores que llevan a la **pérdida de clientes**. Este proyecto tiene como objetivo identificar patrones, tendencias y características clave que influyen en la decisión de los clientes de abandonar el servicio.

### Problema Principal
- 📉 Alta tasa de churn (cancelaciones)
- 💼 Necesidad de retención de clientes
- 🔍 Falta de análisis profundo de causas raíz

## ✅ Lo que se realizó en el Proyecto

### 1. **Extracción de Datos (Extract)**
- Carga y lectura de datasets de clientes de Telecom X
- Importación de múltiples fuentes de datos relacionadas con servicios y características de clientes
- Validación inicial de integridad de archivos

### 2. **Transformación de Datos (Transform)**
- **Limpieza de datos**: manejo de valores faltantes, duplicados y datos inválidos
- **Normalización y estandarización** de variables numéricas y categóricas
- **Creación de nuevas características** (feature engineering) relevantes para el análisis
- **Codificación** de variables categóricas para análisis estadístico
- Validación de integridad y consistencia de datos transformados

### 3. **Carga de Datos (Load)**
- Almacenamiento de datos procesados y limpios
- Preparación de datasets optimizados para análisis posterior
- Documentación de transformaciones realizadas

### 4. **Análisis Exploratorio de Datos (EDA)**
- Análisis descriptivo de las características principales
- Identificación de patrones y tendencias en el comportamiento de clientes
- Detección de anomalías y valores atípicos
- Visualización de relaciones entre variables y su impacto en el churn
- Generación de insights iniciales sobre factores de evasión

### 5. **Hallazgos Clave**
- Identificación de segmentos de clientes de alto riesgo
- Análisis de correlaciones entre características y cancelaciones
- Visualizaciones comprensibles para stakeholders
- Recomendaciones accionables para estrategias de retención

## 🐍 Tecnologías Utilizadas

Este proyecto utiliza **Python 3.8+** y las siguientes bibliotecas:

| Librería | Versión | Propósito |
|----------|---------|----------|
| **pandas** | >= 1.3.0 | Manipulación y análisis de datos |
| **NumPy** | >= 1.21.0 | Computación numérica |
| **Matplotlib** | >= 3.4.0 | Visualización de datos estática |
| **Seaborn** | >= 0.11.0 | Visualización estadística avanzada |
| **Scikit-learn** | >= 0.24.0 | Análisis estadístico y Machine Learning |
| **Jupyter Notebook** | >= 6.4.0 | Análisis interactivo y documentación |

## 📦 Instalación

### Requisitos Previos
- Python 3.8 o superior
- pip (gestor de paquetes de Python)
- Git

### Pasos de Instalación

1. **Clonar el repositorio:**
   ```bash
   git clone https://github.com/SalvatoreSisay/Challenge-Telecome-X.git
   cd Challenge-Telecome-X
   ```

2. **Crear un entorno virtual (opcional pero recomendado):**
   ```bash
   python -m venv venv
   source venv/bin/activate  # En Windows: venv\Scripts\activate
   ```

3. **Instalar las dependencias:**
   ```bash
   pip install -r requirements.txt
   ```

## 📋 Dependencias

Para instalar todas las dependencias requeridas, ejecute:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter notebook
```

O use el archivo `requirements.txt`:
```bash
pip install -r requirements.txt
```

### Versiones Recomendadas
```
pandas>=1.3.0
numpy>=1.21.0
matplotlib>=3.4.0
seaborn>=0.11.0
scikit-learn>=0.24.0
jupyter>=1.0.0
notebook>=6.4.0
```

## 🚀 Cómo Ejecutar el Proyecto

### Opción 1: Ejecutar Jupyter Notebook
1. Inicie Jupyter Notebook en el directorio raíz del proyecto:
   ```bash
   jupyter notebook
   ```

2. Se abrirá una ventana del navegador. Navegue hasta los notebooks y abra el archivo deseado:
   - Notebooks están ubicados en la carpeta `notebooks/`
   - Ejecute las celdas en orden usando `Shift + Enter`

### Opción 2: Ejecutar un Script Específico
Si hay scripts Python en la carpeta `src/`:
```bash
python src/nombre_del_script.py
```

### Estructura del Proyecto
```
Challenge-Telecome-X/
│
├── notebooks/                    # Jupyter Notebooks con análisis
│   ├── 01_EDA_Exploracion.ipynb
│   ├── 02_ETL_Transformacion.ipynb
│   └── 03_Analisis_Churn.ipynb
│
├── data/                         # Datos crudos y procesados
│   ├── raw/                     # Datos sin procesar
│   └── processed/               # Datos limpios y transformados
│
├── src/                          # Código fuente reutilizable
│   └── funciones_utiles.py
│
├── output/                       # Resultados y visualizaciones
│   ├── graficas/
│   └── reportes/
│
├── requirements.txt              # Dependencias del proyecto
├── README.md                     # Este archivo
└── .gitignore
```

## 🛠️ Solución de Problemas y Errores Comunes

### 1. **Error: "ModuleNotFoundError: No module named 'pandas'"**
**Solución:**
```bash
pip install pandas
# O reinstale todas las dependencias
pip install -r requirements.txt --upgrade
```

### 2. **Error: "Jupyter command not found"**
**Solución:**
```bash
pip install jupyter notebook
```

### 3. **Error de Kernel en Jupyter Notebook**
**Solución:**
- Reinicie el kernel: Kernel → Restart
- O ejecute:
```bash
python -m ipykernel install --user
```

### 4. **Problemas de Compatibilidad de Python**
**Solución:**
- Verifique la versión de Python:
  ```bash
  python --version
  ```
- Asegúrese de usar Python 3.8 o superior
- Use un entorno virtual para evitar conflictos

### 5. **Error: "FileNotFoundError: No such file or directory"**
**Solución:**
- Verifique que esté en el directorio correcto del proyecto
- Compruebe que el archivo de datos existe en la ruta especificada
- Use rutas relativas desde la raíz del proyecto

### 6. **Bajo rendimiento o problemas de memoria**
**Solución:**
- Para datasets grandes, procese datos en chunks
- Libere memoria con `del variable_grande` y `gc.collect()`
- Considere usar tipos de datos optimizados en pandas

### 7. **Problemas con visualizaciones en Jupyter**
**Solución:**
```bash
# Agregue esto al inicio del notebook
%matplotlib inline
import matplotlib.pyplot as plt
```

## 📝 Notas Importantes

- ⚠️ **Datos sensibles**: Los datos de clientes son confidenciales. No comparta datasets sin autorización.
- 📊 **Tamaño de datos**: Si el dataset es muy grande (>1GB), considere procesar en lotes.
- 🔄 **Reproducibilidad**: Para resultados consistentes, establezca semillas aleatorias:
  ```python
  import numpy as np
  np.random.seed(42)
  ```

## 📧 Contacto y Soporte

Para preguntas o problemas relacionados con el proyecto, puede:
- Abrir un **issue** en el repositorio de GitHub
- Contactar directamente a través de GitHub

## 👨‍💻 Autor

**SalvatoreSisay** - Challenge Telecom X

---

**¡Gracias por usar este proyecto! 🚀 Juntos descubrimos qué retiene y qué hace que los clientes se vayan.