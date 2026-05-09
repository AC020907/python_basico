# Análisis de Datos de Clientes - Store 1

## 📋 Descripción del Proyecto

Este proyecto forma parte del equipo de análisis de **Store 1** y se enfoca en la limpieza y preparación de datos de clientes para futuros análisis de negocio. El objetivo principal es identificar clientes leales, analizar ingresos por categoría y buscar oportunidades de marketing.

## 🎯 Objetivos

- Limpiar y estandarizar datos de clientes
- Preparar información para análisis de fidelización
- Validar y corregir formatos de datos inconsistentes
- Generar reportes ejecutivos de clientes
- Calcular gastos totales por categorías

## 📊 Conjunto de Datos

**Estructura de datos de clientes:**

- **ID de usuario**: Identificador único del cliente
- **Nombre**: Nombre completo del cliente (requiere limpieza)
- **Edad**: Edad del cliente (conversión a entero)
- **Categorías favoritas**: Lista de categorías de productos preferidas
- **Gastos por categoría**: Lista de montos gastados por categoría

**Volumen de datos:** 10 registros de clientes para procesamiento inicial

## 🛠️ Tecnologías Utilizadas

- **Python 3.9+**
- **Jupyter Notebook**: Entorno de desarrollo
- **Métodos de strings**: strip(), replace(), split()
- **Manejo de excepciones**: try/except para validación

## 🔧 Procesos de Limpieza Implementados

### 1. Limpieza de Nombres

- **Eliminación de espacios**: Uso de `strip()` para quitar espacios iniciales y finales
- **Reemplazo de separadores**: Conversión de guiones bajos (`_`) a espacios
- **Separación de nombres**: División en nombre y apellido usando `split()`

### 2. Validación de Edades

- **Conversión de tipos**: De float a integer para consistencia
- **Manejo de errores**: Validación con try/except para datos no numéricos
- **Mensajes informativos**: Retroalimentación clara para errores de formato

### 3. Organización de Datos

- **Ordenamiento**: Lista ordenada por ID de usuario ascendente
- **Cálculos de gastos**: Suma total de gastos por cliente
- **Formato de reportes**: Cadenas formateadas para presentación ejecutiva

## 📈 Resultados del Procesamiento

### Ejemplo de Transformación:

**Datos originales:**
```
['32415', ' mike_reed ', 32.0, ['ELECTRÓNICA', 'DEPORTE', 'LIBROS'], [894, 213, 173]]
Datos procesados:

['32415', ['mike', 'reed'], 32, ['ELECTRÓNICA', 'DEPORTE', 'LIBROS'], [894, 213, 173]]

Métricas Calculadas:
Total de clientes registrados: 10 clientes
Gasto promedio por cliente: $1,280 (ejemplo usuario mike_reed)
Categorías más populares: ELECTRÓNICA, ROPA, HOGAR
📁 Estructura del Proyecto
store1-analisis/
│
├── New_Project_1_student_version_ESP.ipynb    # Análisis principal
├── README.md                                  # Este archivo
└── data/
    └── usuarios_raw.py                       # Datos originales de clientes
🚀 Cómo Ejecutar el Proyecto
Clonar el repositorio
```bash
