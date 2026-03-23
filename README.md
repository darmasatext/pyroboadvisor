# 🤖 PyRobo Advisor - BMV Strategy Implementation

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)

**Automated investment strategy evaluation on Mexican Stock Exchange (BMV)**

---

## 🇬🇧 English

### Overview

PyRobo Advisor is a personal project exploring the implementation of **Algorithm A1 (Strategy 1)** valuation strategy on the **Mexican Stock Exchange (Bolsa Mexicana de Valores - BMV)**, originally designed for S&P 500 stocks.

### Project Goals

1. ✅ **Replicate A1 algorithm for BMV**: Adapt S&P 500 strategy to Mexican market
2. ✅ **Verify simulation capabilities**: Test if PyRobo Advisor server can run BMV simulations
3. ✅ **Reuse strategy code**: Adapt existing S&P 500 ticker evaluation for BMV tickers
4. ✅ **Extract BMV/IPC tickers**: Automate ticker list retrieval for Mexican stocks
5. ⏳ **Backtesting & validation**: Compare performance vs S&P 500 baseline

### Key Features

- **Market Strategy Evaluation**: `EstrategiaValuacionConSP500` adapted for BMV
- **Backtesting Simulator**: Historical performance testing
- **Data Sources**: Google Sheets integration + market data APIs
- **Multi-market Support**: S&P 500 (baseline) + BMV (experimental)

### Technology Stack

- **Python 3.8+** (Jupyter Notebook)
- **Google Colab** ready (includes Colab badge)
- **Key Libraries**:
  - `pandas` / `numpy` - Data manipulation
  - `gspread` - Google Sheets integration
  - `market.*` - Custom strategy modules (proprietary)
  - `strategyClient` - Strategy execution framework

### Project Structure

```
pyroboadvisor/
├── A1_in_BMV.ipynb          # Main analysis notebook
│   ├── A1 vs S&P500         # Baseline comparison
│   ├── BMV ticker extraction
│   ├── Strategy adaptation
│   └── Simulation results
└── README.md                # This file
```

### Notebook Contents

**`A1_in_BMV.ipynb`** (26 cells):
- **Setup**: Google Colab authentication, library imports
- **Data Loading**: BMV ticker extraction, S&P 500 baseline
- **Strategy Implementation**: A1 algorithm adaptation
- **Simulation**: Backtesting on historical data
- **Results**: Performance metrics, visualization

---

## 🇪🇸 Español

### Resumen

PyRobo Advisor es un proyecto personal que explora la implementación de la estrategia de valuación **Algoritmo A1 (Estrategia 1)** en la **Bolsa Mexicana de Valores (BMV)**, originalmente diseñada para acciones del S&P 500.

### Objetivos del Proyecto

1. ✅ **Replicar algoritmo A1 para BMV**: Adaptar estrategia S&P 500 al mercado mexicano
2. ✅ **Verificar capacidades de simulación**: Probar si servidor PyRobo Advisor puede ejecutar simulaciones BMV
3. ✅ **Reutilizar código de estrategia**: Adaptar evaluación de tickers S&P 500 para tickers BMV
4. ✅ **Extraer tickers BMV/IPC**: Automatizar obtención de lista de acciones mexicanas
5. ⏳ **Backtesting y validación**: Comparar rendimiento vs línea base S&P 500

### Características Principales

- **Evaluación de Estrategia de Mercado**: `EstrategiaValuacionConSP500` adaptada para BMV
- **Simulador de Backtesting**: Pruebas de rendimiento histórico
- **Fuentes de Datos**: Integración Google Sheets + APIs de datos de mercado
- **Soporte Multi-mercado**: S&P 500 (línea base) + BMV (experimental)

### Stack Tecnológico

- **Python 3.8+** (Jupyter Notebook)
- **Google Colab** listo (incluye badge de Colab)
- **Librerías Clave**:
  - `pandas` / `numpy` - Manipulación de datos
  - `gspread` - Integración con Google Sheets
  - `market.*` - Módulos de estrategia personalizados (propietarios)
  - `strategyClient` - Framework de ejecución de estrategias

### Estructura del Proyecto

```
pyroboadvisor/
├── A1_in_BMV.ipynb          # Notebook principal de análisis
│   ├── A1 vs S&P500         # Comparación con línea base
│   ├── Extracción tickers BMV
│   ├── Adaptación de estrategia
│   └── Resultados de simulación
└── README.md                # Este archivo
```

### Contenido del Notebook

**`A1_in_BMV.ipynb`** (26 celdas):
- **Configuración**: Autenticación Google Colab, importación de librerías
- **Carga de Datos**: Extracción tickers BMV, línea base S&P 500
- **Implementación de Estrategia**: Adaptación algoritmo A1
- **Simulación**: Backtesting con datos históricos
- **Resultados**: Métricas de rendimiento, visualización

---

## 🚀 How to Use / Cómo Usar

### Option 1: Google Colab (Recommended)

Click the badge to open in Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/darmasatext/pyroboadvisor/blob/main/A1_in_BMV.ipynb)

### Option 2: Local Jupyter

```bash
# Clone repository / Clonar repositorio
git clone https://github.com/darmasatext/pyroboadvisor.git
cd pyroboadvisor

# Install dependencies / Instalar dependencias
pip install -r requirements.txt

# Launch Jupyter / Iniciar Jupyter
jupyter notebook A1_in_BMV.ipynb
```

### Prerequisites / Requisitos

```python
# Core libraries / Librerías principales
pip install pandas numpy jupyter gspread google-auth

# Note: market.* modules are proprietary
# Nota: módulos market.* son propietarios
```

---

## 📊 Strategy Overview / Resumen de Estrategia

### Algorithm A1 (Strategy 1)

**Original Market:** S&P 500  
**Adapted For:** BMV (Bolsa Mexicana de Valores)

**Core Concept:**
Valuation-based stock selection using fundamental analysis combined with market timing indicators.

**Key Components:**
1. **Ticker Selection**: BMV/IPC constituent extraction
2. **Valuation Metrics**: Price-to-earnings, growth rates, fundamentals
3. **Backtesting Engine**: Historical simulation framework
4. **Performance Analysis**: Risk-adjusted return metrics

**Adaptation Challenges:**
- Lower liquidity in BMV vs S&P 500
- Different market hours and trading patterns
- Currency considerations (MXN vs USD)
- Smaller universe of stocks

---

## ⚠️ Important Notes / Notas Importantes

### 🇬🇧 English

**Disclaimer:**
- This is a **research/educational project**, not investment advice
- Strategy performance is historical and does not guarantee future results
- The `market.*` modules are proprietary and not included in this repository
- Mexican stock market data may require specific data provider subscriptions

**Status:**
- Last active: July 2025
- Current state: Experimental / proof-of-concept
- Not production-ready

### 🇪🇸 Español

**Descargo de responsabilidad:**
- Este es un **proyecto de investigación/educativo**, no asesoría de inversión
- El rendimiento de la estrategia es histórico y no garantiza resultados futuros
- Los módulos `market.*` son propietarios y no están incluidos en este repositorio
- Los datos del mercado mexicano pueden requerir suscripciones a proveedores específicos de datos

**Estado:**
- Última actividad: Julio 2025
- Estado actual: Experimental / prueba de concepto
- No listo para producción

---

## 🔗 Related Projects / Proyectos Relacionados

**For production-ready financial data pipelines, see:**

- [sp500-finance-etl](https://github.com/darmasatext/sp500-finance-etl) - S&P 500 ETL pipeline to BigQuery (Python, Cloud Run)
- [rappi-data-challenges](https://github.com/darmasatext/rappi-data-challenges) - Data Science technical challenges

---

## 📜 License / Licencia

MIT License - See [LICENSE](./LICENSE) file for details.

---

## 📧 Contact / Contacto

**Diego Armas**  
GitHub: [@darmasatext](https://github.com/darmasatext)  
Email: diegoarmastexta@gmail.com

---

## 🏷️ Keywords / Palabras Clave

`python` `jupyter` `finance` `trading-strategy` `backtesting` `bmv` `mexico` `stock-market` `algorithmic-trading` `investment-strategy` `data-analysis` `google-colab`

---

**Last Updated / Última Actualización:** March 2026  
**Original Development / Desarrollo Original:** 2024-2025  
**Status / Estado:** Archived (research project) / Archivado (proyecto de investigación)
