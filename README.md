# 🤖 Chatbot IA Multimodelo

Un chatbot inteligente y multifuncional que permite **conversar, traducir y resumir textos** utilizando **diferentes modelos de inteligencia artificial** conectados mediante las **APIs de OpenRouter y Groq**.

Su objetivo es ofrecer una experiencia conversacional fluida, natural y adaptable a múltiples tareas y lenguajes, todo desde una interfaz moderna desarrollada con **Gradio**.

---

## 🚀 Características principales

- 🧠 **Multimodelo:** puedes elegir entre varios modelos de IA:
  - **Llama 3 (Meta)**
  - **Gemini 2.5 Pro (Google)**
  - **Grok (Groq API)**
  - **DeepSeek V3.2**
  - **ChatGPT 5 (OpenAI)**

- 💬 **Tareas disponibles:**
  - **Conversar:** mantiene diálogos con tono humano, emocional y natural.
  - **Traducir:** traduce entre varios idiomas de manera precisa.
  - **Resumir:** resume textos largos, extrayendo los puntos más importantes.

- 🧠 **Memoria de conversación:** guarda el historial de chat en `history.json` para mantener coherencia entre mensajes.

- 📄 **Lectura de archivos:** permite procesar **PDF, Word y CSV**.

- 🎨 **Interfaz personalizada con Gradio** y diseño **Glassmorphism (efecto blur)**.

- ⏱️ **Muestra el tiempo de inferencia** (respuesta del modelo).

---

## 🧰 Tecnologías utilizadas

| Tipo | Herramientas |
|------|---------------|
| Lenguaje principal | Python 3 |
| Interfaz gráfica | Gradio |
| APIs de modelos IA | OpenRouter API, Groq API |
| Procesamiento de documentos | PyPDF2, python-docx, pandas |
| Comunicación HTTP | requests |
| Persistencia | JSON local |
| Estilos | CSS personalizado |

---

## ⚙️ Instalación

### 1️⃣ Clonar el repositorio
```bash
git clone https://github.com/tuusuario/chatbot_ia_multimodelo.git
cd chatbot_ia_multimodelo
```

### 2️⃣ Instalar dependencias
```bash
pip install -r requirements.txt
```

### 3️⃣ Configurar las claves API
Crea un archivo `.env` o define las variables de entorno en tu terminal:
```bash
export OPEN_ROUTER_API_KEY="tu_clave_openrouter"
export GROQ_API_KEY="tu_clave_groq"
```

> 💡 También puedes reemplazar las claves directamente dentro del archivo `chatbot_ia_multifuncional.py` si lo estás ejecutando en Colab.

---

## 🧠 Uso

### Ejecución local
```bash
python chatbot_ia_multifuncional.py
```

Se abrirá una interfaz web con **Gradio**, donde podrás:

1. Seleccionar la **tarea** (resumir, traducir o conversar).  
2. Escoger el **modelo de IA** (Llama, Gemini, Grok, DeepSeek o ChatGPT-5).  
3. Ingresar tu texto o archivo.  
4. Visualizar la respuesta y el tiempo de ejecución.

---

## 💬 Ejemplos de uso

- **Resumir**
  > “Resume este texto sobre la evolución de la inteligencia artificial.”

- **Traducir**
  > Entrada: *English* → Salida: *Español*  
  > “Translate this paragraph about renewable energy.”

- **Conversar**
  > “Hola, ¿cómo te sientes hoy?”  
  *(El chatbot responderá con un tono natural y cercano.)*

---

## 🧩 Estructura del proyecto

```
📂 chatbot_ia_multimodelo/
│
├── chatbot_ia_multifuncional.py   # Código principal (backend + interfaz)
├── requirements.txt               # Librerías requeridas
├── history.json                   # Archivo donde se guarda el historial del chat
└── README.md                      # Documentación del proyecto
```

---

## 🧑‍💻 Autor

**Camilo Andrés Ramos Cotes**  
Desarrollador y creador del chatbot multimodelo.  
🎵 Artista y programador apasionado por la inteligencia artificial aplicada a la creatividad.

---

## 📜 Licencia

Este proyecto se distribuye bajo la licencia **MIT**, permitiendo su uso, modificación y distribución con atribución al autor original.

---

## ⭐ Recomendaciones

- Añadir más modelos (Claude, Mistral, Mixtral, etc.).
- Integrar reconocimiento de voz y respuesta hablada (text-to-speech).
- Implementar versión web o de escritorio con autenticación.
- Si te gusta este proyecto, ¡no olvides dejar una ⭐ en GitHub!

---

**Versión:** 1.0  
**Última actualización:** Octubre 2025


🧩 Reflexión técnica

Durante el desarrollo del Chatbot IA Multimodelo, se logró integrar múltiples APIs de inteligencia artificial en una sola interfaz funcional y flexible, aprendiendo sobre la comunicación entre servicios externos, el manejo de claves API, y la gestión dinámica de tareas como traducción, resumen y conversación.
El uso de Gradio facilitó la creación de una interfaz interactiva sin necesidad de frameworks complejos de frontend, reforzando la comprensión del flujo entre backend y visualización.

Entre los principales límites encontrados se destacan:

Las restricciones de uso y latencia de algunas APIs gratuitas.

La dependencia de conexión a Internet para cada petición.

La necesidad de manejar mejor los errores de respuesta y tiempos de espera de los modelos.

Como posibles mejoras, se plantea:

Incorporar procesamiento local o en caché para reducir dependencias externas.

Agregar reconocimiento y síntesis de voz para hacerlo totalmente conversacional.

Incluir más modelos (como Claude o Mistral) y un sistema de autenticación para usuarios.

Optimizar la experiencia visual con temas y animaciones adaptativas.

En conclusión, el proyecto permitió afianzar habilidades técnicas en integración de APIs, desarrollo modular y diseño de interfaces interactivas con IA, abriendo la puerta a futuras versiones más potentes e inteligentes.
