# Autonomous Resource & Communications Pipeline
An enterprise-grade, serverless AI orchestration pipeline that automates meeting scheduling and professional communication using a dual-LLM architecture.

## 🚀 The Problem
Standard automation often fails at handling unstructured human intent. This project solves that by using High-Inference LPUs to bridge the gap between "natural language emails" and "strictly typed calendar data."

## 🧠 Architecture & Tech Stack
- **Orchestration:** n8n (Serverless Workflow Engine)
- **AI Brain:** Groq LPU (Llama 3.1 8B Instant)
- **APIs:** Google Calendar API, Gmail API
- **Protocol:** Direct REST/HTTP Integration (Bypassing standard no-code wrappers for absolute control)

### Key Features:
* **Zero-Touch Scheduling:** Automatically parses incoming emails for intent, dates, and times without human intervention.
* **Dual-Agent Logic:** * **Agent 1 (Extractor):** Performs entity extraction to convert unstructured text into valid JSON.
    * **Agent 2 (Writer):** Generates context-aware, professional email confirmations based on the scheduled event.
* **LPU Optimization:** Utilizes Groq's low-latency inference to achieve end-to-end execution in under 4 seconds.

## 🛠️ Installation & Setup
1. **Clone the repo:** `git clone https://github.com/NallaSumang/ai-resource-manager.git`
2. **Import Workflow:** Open n8n, click 'Import from File', and select `workflow.json`.
3. **Configure Credentials:**
    - Add your **Groq API Key** in the HTTP Request nodes.
    - Connect your **Google OAuth2** credentials for Gmail and Calendar.
4. **Deploy:** Hit "Execute" and send a test email to your connected account.

## 📊 Business Impact
* **Reduced Latency:** Direct API integration reduced response time by 60% compared to standard AI wrappers.
* **Operational Efficiency:** Eliminates the need for manual calendar management and back-and-forth emailing.
