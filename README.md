# 🤖 E-commerce AI Support Agent (n8n + Gemini)

An automated customer support Telegram bot for e-commerce, built with **n8n** and powered by **Google Gemini**. The bot acts as an intelligent sales assistant, answering product-related questions, helping with orders, and maintaining conversational context.

---

## ✨ Features

* **Telegram Integration:** Seamless two-way communication using native n8n Telegram triggers and actions.
* **Context-Aware AI:** Uses LangChain-based **AI Agent** architecture with a memory buffer to remember conversation history.
* **LLM Engine:** Powered by **Google Gemini** for fast, cost-effective, and natural responses.
* **Custom Persona & Knowledge:** Configurable system prompt tailored to store policies, pricing, catalog details, and FAQs.

---

## 🛠 Tech Stack

* **Workflow Engine:** [n8n](https://n8n.io/)
* **LLM:** Google Gemini (via `@n8n/n8n-nodes-langchain.lmChatGoogleGemini`)
* **Framework:** LangChain Nodes in n8n (Agent + Window Buffer Memory)
* **Messaging Platform:** Telegram Bot API

---

## 📐 Architecture

### Workflow Overview:
1. **Telegram Trigger:** Listens for incoming user messages in real time.
2. **AI Agent Node:** Processes the user query using the predefined store persona and guidelines.
3. **Google Gemini Model:** Generates dynamic, context-relevant responses.
4. **Simple Memory:** Maintains chat history for contextual multi-turn conversations.
5. **Send Text Message:** Dispatches the generated response back to the user on Telegram.

---

## 🚀 Quickstart & Setup

### Prerequisites
* A running **n8n** instance (Cloud or Self-hosted Docker).
* A **Telegram Bot Token** (obtainable via [@BotFather](https://t.me/botfather)).
* A **Google Gemini API Key** (obtainable via [Google AI Studio](https://aistudio.google.com/)).

### Installation
1. Clone this repository or download the `aiAgentTGBot.json`
