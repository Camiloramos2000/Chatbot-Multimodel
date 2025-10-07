# 🤖 Multi-Model AI Chatbot

An intelligent and multifunctional chatbot that can **converse, translate, and summarize text** using **multiple artificial intelligence models** connected through the **OpenRouter** and **Groq APIs**.

Its goal is to deliver a fluent, natural, and adaptive conversational experience for various tasks and languages, all through a modern interface built with **Gradio**.

---

## 🚀 Main Features

- 🧠 **Multi-model:** choose from several AI models:
  - **Llama 3 (Meta)**
  - **Gemini 2.5 Pro (Google)**
  - **Grok (Groq API)**
  - **DeepSeek V3.2**
  - **ChatGPT 5 (OpenAI)**

- 💬 **Available tasks:**
  - **Conversation:** maintains a natural, emotional, and human-like dialogue.  
  - **Translation:** translates between multiple languages accurately.  
  - **Summarization:** condenses long texts, extracting key points.  

- 🧠 **Conversation memory:** stores chat history in `history.json` to maintain message coherence.  

- 📄 **File reading:** supports processing of **PDF, Word, and CSV** files.  

- 🎨 **Custom interface with Gradio** and a **Glassmorphism (blur effect)** design.  

- ⏱️ **Displays model inference time** (response duration).  

---

## 🧰 Technologies Used

| Type | Tools |
|------|-------|
| Main language | Python 3 |
| GUI | Gradio |
| AI model APIs | OpenRouter API, Groq API |
| Document processing | PyPDF2, python-docx, pandas |
| HTTP communication | requests |
| Data persistence | Local JSON |
| Styling | Custom CSS |

---

## ⚙️ Installation

### 1️⃣ Clone the repository
```bash
git clone https://github.com/Camiloramos2000/Chatbot-Multimodel.git
cd Chatbot-Multimodel
2️⃣ Install dependencies
bash
Copiar código
pip install -r requirements.txt
3️⃣ Set up API keys
Create a .env file or set the environment variables in your terminal:

bash
Copiar código
export OPEN_ROUTER_API_KEY="your_openrouter_key"
export GROQ_API_KEY="your_groq_key"
💡 You can also replace the keys directly in the chatbot_ia_multifuncional.py file if running on Google Colab.

🧠 Usage
Run locally
bash
Copiar código
python chatbot_ia_multifuncional.py
A Gradio web interface will open where you can:

Select a task (summarize, translate, or chat).

Choose the AI model (Llama, Gemini, Grok, DeepSeek, or ChatGPT-5).

Enter your text or upload a file.

View the model’s response and inference time.

💬 Example Prompts
Summarization

“Summarize this text about the evolution of artificial intelligence.”

Translation

Input: English → Output: Spanish
“Translate this paragraph about renewable energy.”

Conversation

“Hi, how are you feeling today?”
(The chatbot will reply naturally and emotionally.)

🧩 Project Structure
bash
Copiar código
📂 chatbot_ia_multimodelo/
│
├── chatbot_ia_multifuncional.py   # Main code (backend + interface)
├── requirements.txt               # Required libraries
├── history.json                   # File that stores chat history
└── README.md                      # Project documentation
🧑‍💻 Author
Camilo Andrés Ramos Cotes
Developer and creator of the multi-model chatbot.
🎵 Artist and programmer passionate about artificial intelligence applied to creativity.

📜 License
This project is distributed under the MIT License, allowing free use, modification, and distribution with proper attribution to the original author.

⭐ Recommendations
Add more models (Claude, Mistral, Mixtral, etc.).

Integrate voice recognition and text-to-speech for full conversational capability.

Implement a web or desktop version with authentication.

If you like this project, don’t forget to ⭐ it on GitHub!

Version: 1.0
Last update: October 2025

🧩 Technical Reflection
During the development of the Multi-Model AI Chatbot, multiple AI APIs were successfully integrated into a single, flexible interface.
This process involved learning how to manage communication between external services, handle API keys securely, and dynamically perform tasks such as translation, summarization, and conversation.

The use of Gradio made it possible to create an interactive interface without the need for complex frontend frameworks, reinforcing the understanding of how backend logic connects with visualization layers.

Main Limitations
Usage limits and latency from some free APIs.

Full dependence on an internet connection for every request.

Need for better error handling and timeout management.

Possible Improvements
Add local or cached processing to reduce external dependencies.

Integrate speech recognition and synthesis for a fully conversational experience.

Include more models (Claude, Mistral) and a user authentication system.

Enhance the visual experience with adaptive themes and animations.

In conclusion, this project strengthened technical skills in API integration, modular development, and building interactive AI interfaces — opening the door to more advanced and powerful future versions.
