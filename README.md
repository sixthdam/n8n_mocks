# 🌐 n8n_mocks
## Hoja de Ruta: Dominio de n8n y Automatización

Este documento demuestra el uso y construcción de workflows básicos hasta sistemas autónomos con uso de Inteligencia Artificial.

---

## 🟢 Nivel Fácil: Fundamentos y Consumo de Datos (1–5)

### 🎯 Objetivo
Comprender el manejo de datos, nodos básicos y consumo de APIs.

---

### Flujo con datos estáticos
- **Práctica:** Uso del nodo `Set` para definir variables (nombre, ciudad).
- **Resultado:** Visualización de datos al final del flujo.

---

### Consumo de API pública 🌐
- **Práctica:** Uso de `HTTP Request` para consultar APIs simples.
- **Resultado:** Lectura de JSON y visualización de datos.

---

### Transformación de datos 🔄
- **Práctica:** Modificar resultados.
- **Resultado:** Uso de nodos `Set` o `Code`.

---

### Ejecución programada ⏰
- **Práctica:** Automatización con `Cron`.
- **Resultado:** Ejecución sin intervención humana.

---

### Persistencia de datos 💾
- **Práctica:** Guardar datos en Google Sheets.
- **Resultado:** Registro exitoso en fuente externa.

---

## 🟡 Nivel Medio: Lógica y Procesos Dinámicos (6–10)

### 🎯 Objetivo
Integrar múltiples fuentes de datos y aplicar lógica condicional.

---

### Parámetros dinámicos
- **Práctica:** Uso de variables en Query Params.
- **Resultado:** Consultas personalizadas.

---

### Combinación de APIs 🔗
- **Práctica:** Unir datos de múltiples fuentes.
- **Resultado:** Dominio del nodo `Merge`.

---

### Filtrado de datos 🔍
- **Práctica:** Aplicar condiciones a resultados.
- **Resultado:** Uso de nodos `IF`.

---

### Manejo de errores ⚠️
- **Práctica:** Crear flujos alternativos ante fallos.
- **Resultado:** Mayor robustez del sistema.

---

### Decisiones automatizadas 🤖
- **Práctica:** Lógica basada en datos reales.
- **Resultado:** Automatización con bifurcaciones.

---

## 🔴 Nivel Difícil: IA y Sistemas Completos (11–15)

### 🎯 Objetivo
Implementar IA y construir sistemas autónomos reales.

---

### IA + API Data 🧠
- **Práctica:** Enviar datos a IA para generar resúmenes.
- **Resultado:** Integración de IA con contenido.

---

### Clasificación por IA 📊
- **Práctica:** Análisis de sentimiento o categoría.
- **Resultado:** Creación de prompts de clasificación.

---

### Salida estructurada 🧾
- **Práctica:** Forzar respuestas JSON.
- **Resultado:** Parsing estructurado.

---

### Decisiones basadas en IA 🧠⚡
- **Práctica:** Ramificar flujo según resultados.
- **Resultado:** Automatización inteligente.

---

### Sistema Autónomo Final 🚀
- **Práctica:** Cron → API → IA → Clasificación → Almacenamiento.
- **Resultado:** Sistema completamente automatizado.

---

## 🧰 Recursos y Herramientas

### 🔗 APIs de prueba
- GNews → Noticias
- Open-Meteo Geocoding → Coordenadas por ciudad

---

## 🗄️ Destinos de datos
- Google Sheets

---

## 🤖 Inteligencia Artificial
- Google Gemini 3.1 flash-lite-preview
- Integraciones locales en n8n

---

## 🚀 Cómo ejecutar el proyecto

Este proyecto está diseñado para ejecutarse en **n8n**, utilizando workflows en formato JSON.
```
    git clone https://github.com/sixthdam/n8n_mocks.git
```

---

### 🧩 Requisitos

- Tener instalado **n8n** (local o en la nube)
- Cuenta de **Google Sheets** conectada
- API Key de:
  - [GNews](https://gnews.io/)
- Credenciales de:
  - Google Gemini (configuradas en n8n)

---

### 📥 Importar el workflow

1. Abre n8n
2. Ve a **Workflows**
3. Haz clic en **Import**
4. Pega el JSON del workflow
5. Guarda el flujo

---

Antes de ejecutar, debes configurar:

### 📰 GNews API
Se usa como Query Param:
```
apikey = TU_API_KEY
```
---
### 🤖 Google Gemini
- Credentials → Google Gemini (PaLM)
- Asegúrate de seleccionar el modelo en el nodo LLM

---

## 👨‍💻 Autor

🤖 [Karina Méndez](https://github.com/sixthdam/)
