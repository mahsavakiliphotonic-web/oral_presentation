# 🌿 AgriGuide: AI-Powered Precision Plant Pathology

**AgriGuide** is an advanced AI-assisted tool designed to bridge the gap between complex agricultural science and practical farming. By leveraging **Retrieval-Augmented Generation (RAG)** and **Multimodal LLMs**, AgriGuide provides real-time, localized crop disease diagnosis and expert-level treatment advice based on authoritative scientific literature.

---

## 🚀 Features

- **Multimodal Diagnosis:** Upload images of infected crops for immediate AI-driven identification.
- **RAG-Powered Intelligence:** Unlike general AI, AgriGuide consults specialized compendiums (e.g., APS, FAO) to provide scientifically validated answers.
- **Localized Detection:** Tailored alerts and management strategies based on regional pest status protocols.
- **Expert Assistant:** A conversational interface for farmers and researchers to explore treatment options and prevention strategies.

---

## 🛠 Tech Stack

Based on modern development standards, this project utilizes a high-performance stack:

### Frontend
- **Framework:** [Next.js](https://nextjs.org/) (React-based)
- **Language:** [TypeScript](https://www.typescriptlang.org/) for type-safe UI development.
- **Styling:** [Tailwind CSS](https://tailwindcss.com/) & [Shadcn/UI](https://ui.shadcn.com/) for a responsive, modern interface.

### Backend & AI
- **Language:** [Python](https://www.python.org/) (The core of AI and data processing).
- **LLM Provider:** [Google Gemini 1.5 Flash](https://aistudio.google.com/) for multimodal processing and large context windows.
- **RAG Framework:** Custom pipeline for document chunking and vector retrieval.
- **Data Sources:** Scientific literature from **APS (American Phytopathological Society)** and **FAO**.

---

## 📂 Project Structure

```text
├── frontend/           # Next.js & TypeScript UI
│   ├── components/     # UI elements (Shadcn/UI)
│   └── pages/          # App routing and Chat interface
├── backend/            # Python AI & RAG logic
│   ├── scripts/        # PDF processing & Embedding scripts
│   └── main.py         # API Gateway for communication
├── data/               # Scientific PDF repository (FAO, APS)
└── .env                # Secure API Key management
📖 Methodology (The RAG Process)
Document Ingestion: High-authority PDFs (like the Compendium of Potato Diseases) are processed and indexed.

User Query: A farmer uploads a photo or asks a question.

Retrieval: The system searches the indexed scientific data for relevant symptoms and treatments.

Generation: Gemini synthesizes the "User Image" + "Scientific Data" to provide a precise diagnosis.
