# Internal Docs Q&A Agent

### 🤖 AI Agent Hackathon Project by Team Brainstormers

This project is an AI-powered internal documentation Q&A agent, developed by Team Brainstormers for the **AI Agents Hackathon by Product Space**. It solves the common problem of employees wasting time searching for internal information by providing instant, accurate, and source-cited answers from a centralized knowledge base.

The agent uses a **Retrieval-Augmented Generation (RAG)** pipeline to intelligently answer questions based on the provided documents, ensuring responses are grounded in fact and not fabricated.

## ✨ Features

* **Intelligent Q&A:** Ask natural language questions and get concise, accurate answers from the knowledge base.

* **Custom Knowledge Base:** Easily upload your own `.txt` files to index and create a custom knowledge base on the fly.

* **Source Citation:** Every AI-generated answer includes citations to the specific document chunks used, providing transparency and building trust.

* **Persistent Chat History:** Your conversations are automatically saved using **Firebase Firestore**, so you never lose your progress.

* **Dynamic UI:** A modern, interactive user interface with a live gradient background and elegant animations creates an impressive and engaging user experience.

* **AI Model Selection:** Toggle between different AI models (e.g., Gemini 2.5 Flash, Gemini 1.5 Pro) to test and compare their performance.

* **Responsive Design:** The application is fully responsive and designed to work seamlessly on both desktop and mobile devices.

## ⚙️ How It Works (The RAG Pipeline)

1. **Document Ingestion:** You upload a `.txt` file, which the application reads and splits into smaller, manageable chunks of text.

2. **Embedding & Indexing:** Each text chunk is converted into a numerical vector (**embedding**) that represents its semantic meaning. These embeddings are then stored in a database (an in-memory store for this demo).

3. **Query & Retrieval:** When a user asks a question, the question is also converted into an embedding. The system then performs a vector similarity search to find the most relevant document chunks from the indexed knowledge base.

4. **Generation:** The retrieved document chunks are sent as context to a large language model (LLM). The LLM's role is to act as a smart editor, synthesizing the information from the provided context to formulate a coherent and cited answer.

## 🚀 Getting Started

This project is a single-file web application, so you can run it directly in your browser.

1. Clone this repository:

   ```
   git clone [https://github.com/siddhu1430/Internal-Q-A-Agent.git](https://github.com/siddhu1430/Internal-Q-A-Agent.git)
   
   
   ```

2. Open the `Internal Q&A Agent.html` file in your preferred web browser.

**Note:** The application uses the Gemini API. You will need a valid API key to run it. The placeholder in the code should be replaced with your own key.

## 🤝 Team Brainstormers

This project was a collaborative effort by:

* **Siddhant Deshmukh**

* **Atharv Bangle**

*Contributed a problem statement solution in the AI Agent Hackathon by Product Space.*
