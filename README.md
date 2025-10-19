# CatAI---AI-Powered-Cataract-Detection-using-n8n-and-Google-Gemini
# 👁️ CatAI — AI-Powered Cataract Detection using n8n + Google Gemini

CatAI is an **AI automation workflow** built using **n8n** that detects and classifies **cataract stages** from eye images.  
It uses **Google Gemini (PaLM)** for intelligent image reasoning and a **Structured Output Parser** to produce medical-grade JSON results.

---

## 🚀 Features

- 🧠 AI-powered cataract stage detection (Early, Immature, Mature, Hypermature)
- 🔍 Predicts **intensity score** and **confidence levels**
- 📦 Structured, machine-readable output (JSON)
- 🌐 Webhook endpoint for image upload
- ⚡ No backend coding required — built entirely with **n8n** and **LangChain nodes**
- 🔄 Extendable with GPT or Vision APIs

---

## 🧩 Tech Stack

| Component | Purpose |
|------------|----------|
| **n8n** | Workflow automation platform |
| **Google Gemini API** | Language & vision model |
| **LangChain Nodes** | For prompt handling & output structuring |
| **Structured Output Parser** | Enforces consistent JSON schema |
| **Webhook Trigger** | Accepts image uploads from users |

---

## ⚙️ Workflow Overview

```mermaid
graph TD;
    A[Webhook Trigger] --> B[Google Gemini Model];
    B --> C[AI Agent Node (Cataract Analysis Prompt)];
    C --> D[Structured Output Parser];
    D --> E[JSON Response to User];
