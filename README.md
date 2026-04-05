#  Análisis de Métricas de Usuario y Costos de Marketing – Showz

##  Descripción del Proyecto
Análisis integral del comportamiento de usuarios y rentabilidad de las estrategias de marketing para Showz, una plataforma de venta de entradas de eventos. El proyecto evalúa cómo los usuarios interactúan con el servicio, cuándo realizan su primera compra y qué tan rentable es cada canal de adquisición de clientes.

---
##  Objetivos
- Analizar el comportamiento y actividad de los usuarios en la plataforma
- Determinar el tiempo entre el registro y la primera compra
- Calcular el valor de vida del cliente (LTV) por cohorte
- Evaluar la rentabilidad de los canales de marketing mediante CAC y ROMI

---

##  Herramientas y Librerías

| Librería | Uso |
|---|---|
| `Pandas` | Manipulación y análisis de datos |
| `NumPy` | Operaciones numéricas y cálculo de métricas |
| `Matplotlib` | Visualizaci

##  Metodología

### 1. Limpieza y Preprocesamiento
- Estandarización de columnas a formato snake_case
- Conversión de columnas de fecha a formato datetime
- Cálculo de variables derivadas: duración de sesión, mes y año de inicio

### 2. Análisis de Comportamiento de Usuarios
Métricas calculadas para entender la actividad en la plataforma:

| Métrica | Valor |
|---|---|
| DAU (Usuarios Activos Diarios) | 907 |
| WAU (Usuarios Activos Semanales) | 5.716 |
| MAU (Usuarios Activos Mensuales) | 23.228 |
| Factor de Adherencia (DAU/MAU) | 0.039 |

- **Sesiones por mes:** Análisis de número de sesiones y usuarios activos por mes
- **Duración de sesión:** El comportamiento de compra ocurre entre 17 y 23 horas tras la primera visita
- **Tasa de retención por cohorte:** Visualización mediante mapa de calor por mes de primera sesión

### 3. Análisis de Compras
- Número de compras por mes con visualización de barras
- Ingreso promedio por mes y comparación con volumen de pedidos
- Identificación de estacionalidad: mayor actividad en el primer y último trimestre del año

### 4. Valor de Vida del Cliente (LTV)
- Cálculo del LTV por cohorte basado en el mes de primera compra
- Tabla pivote de LTV acumulado por ciclo de vida del cliente
- Mapa de calor para identificar cohortes más rentables

### 5. Análisis de Marketing

####  Costo de Adquisición de Clientes (CAC)
- Cálculo del CAC por fuente de adquisición
- Clasificación de usuarios como **rentables** o **no rentables** según LTV vs CAC
- Gráfico de rentabilidad por usuario (pie chart)

####  Retorno sobre Inversión en Marketing (ROMI)
- Cálculo del ROMI = LTV / CAC por cohorte y ciclo de vida
- Mapa de calor del ROMI por mes de primera compra

---

## 📊 Hallazgos Principales
- El factor de adherencia de 0.039 indica que los usuarios no interactúan de forma constante con la plataforma
- Los meses con mayor número de usuarios y sesiones son enero y los últimos tres meses del año
- El 66% de los usuarios resultaron **no rentables** para la empresa según el análisis CAC vs LTV
- La tasa de retención se mantiene estable en los primeros meses pero disminuye progresivamente
- El comportamiento de compra ocurre entre **17 y 23 horas** después de la primera visita

---

## ✅ Recomendaciones
- Implementar estrategias de reactivación para mejorar el factor de adherencia
- Optimizar la inversión en los canales de adquisición con mayor ROMI
- Diseñar incentivos para convertir usuarios no rentables en clientes recurrentes
- Reforzar campañas en los períodos de baja actividad (febrero a agosto)





