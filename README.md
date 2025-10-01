# 💔 Breakup Recovery Squad: Tu Equipo de Recuperación Asistido por IA

Esta aplicación web es una herramienta de apoyo emocional diseñada para ayudar a los usuarios a navegar y procesar las emociones complejas que siguen a una ruptura sentimental. Utiliza el poder de la Inteligencia Artificial de Google Gemini para ofrecer planes de recuperación personalizados, apoyo empático y perspectivas honestas.

## 🌟 Características Principales

* **Agente Terapeuta Empático:** Ofrece apoyo emocional y valida los sentimientos del usuario.
* **Agente de Cierre:** Ayuda a crear mensajes de cierre emocional para liberar sentimientos no expresados.
* **Planificador de Rutinas:** Genera desafíos de recuperación y planes de autocuidado de 7 días.
* **Perspectiva Honesta:** Proporciona retroalimentación objetiva y directa para impulsar el avance.

## 🔒 Guardrails de Seguridad Implementados

El proyecto cuenta con un sistema de triple capa para garantizar la seguridad y privacidad del usuario:

1.  **Bloqueo de Entrada:** El sistema **detiene inmediatamente la ejecución** si detecta **Información de Identificación Personal (PII)** (correos, teléfonos, cédulas) o **Lenguaje Grosero** en el mensaje de entrada.
2.  **Limpieza de PII:** Los datos personales detectados son eliminados antes de ser procesados por el modelo.
3.  **Instrucciones del Sistema (System Instructions):** Se garantiza que la respuesta del modelo Gemini mantenga un tono respetuoso y no aborde temas de riesgo (autolesión, actividades ilegales, etc.).

## 🛠️ Tecnologías Utilizadas

* **Modelo de IA:** Gemini 2.5 Flash (a través de la librería `google-genai`).
* **Frontend:** Streamlit.
* **Librerías de Utilidad:** `ddgs` (para búsquedas, aunque actualmente no está implementada en la lógica final), `re`.

## ⚙️ Cómo Ejecutar Localmente (o en Colab)

### Requisitos

Necesitas una **Clave API de Gemini**.

### Pasos de Ejecución

1.  **Clonar el Repositorio:**
    ```bash
    git clone [https://github.com/tu_usuario/tu_repositorio.git](https://github.com/tu_usuario/tu_repositorio.git)
    cd tu_repositorio
    ```
2.  **Instalar Dependencias:**
    ```bash
    pip install google-genai streamlit
    ```
3.  **Ejecutar la Aplicación:**
    ```bash
    streamlit run app.py
    ```
4.  **Uso:** Abre la URL que aparece en tu terminal (usualmente `http://localhost:8501`), **ingresa tu Clave API en la barra lateral**, y comienza a compartir tus sentimientos.
