---

title: "TeaCareAI"

description: "AI-powered tea disease detection, treatment recommendation and recovery tracking system."

date: "Jun 2025"

demoURL: "https://github.com/visharaaa/TeaCareAI"

repoURL: "https://github.com/visharaaa/TeaCareAI"

---

TeaCareAI is a full-stack AI-powered platform designed to help tea farmers and agronomists detect and manage tea plantation diseases. The system combines computer vision, Retrieval-Augmented Generation (RAG), and deep learning to identify diseases from tea leaf images, provide context-aware treatment recommendations, and track plant recovery over time.

The project was developed with a focus on Sri Lankan tea plantations, combining disease detection with localized agricultural knowledge and field-level analytics.

## 🌱 Features

* ✅ Tea leaf image verification
* ✅ AI-powered disease detection using YOLOv8
* ✅ Infection severity estimation
* ✅ Retrieval-Augmented Generation (RAG) for treatment recommendations
* ✅ Localized agricultural knowledge base
* ✅ Natural language treatment explanations using Llama 3.1
* ✅ Treatment and recovery tracking
* ✅ Deep learning-based recovery prediction
* ✅ Field management and crop analytics
* ✅ PostgreSQL database integration
* ✅ Flask-based backend
* ✅ Docker support

## 🤖 AI & Machine Learning

### Disease Detection

A YOLOv8-based computer vision model identifies tea leaf diseases from uploaded images and estimates the percentage of the leaf affected by the disease.

### Treatment Recommendation

A RAG pipeline combines ChromaDB with BGE-small-en-v1.5 embeddings to retrieve relevant agricultural knowledge from a localized treatment repository. Llama 3.1 is then used to convert the retrieved information into practical treatment guidance.

### Recovery Tracking

A TensorFlow/Keras neural network analyzes sequential plant health data to determine whether a plant is improving, deteriorating, stable, or being newly tracked.

## 🏗️ Architecture

TeaCareAI uses a modular Flask backend connecting independent machine learning services with a PostgreSQL data layer.

The main components include:

* **Computer Vision:** YOLOv8 / PyTorch
* **RAG:** ChromaDB + SentenceTransformers
* **LLM:** Llama 3.1 via Ollama
* **Recovery Model:** TensorFlow / Keras
* **Backend:** Flask
* **Database:** PostgreSQL
* **Deployment:** Docker

## 🔄 User Flow

1. Create an account and manage tea fields.
2. Upload a tea leaf image for analysis.
3. Verify that the uploaded image contains a tea leaf.
4. Detect the disease and estimate infection severity.
5. Retrieve relevant agricultural knowledge using RAG.
6. Generate context-aware treatment recommendations.
7. Track subsequent scans to monitor recovery.
8. Analyze plant and field-level information over time.

## 📊 Project Highlights

* Built as a modular full-stack AI system rather than a standalone classification model.
* Combined computer vision, RAG, LLMs, and predictive analytics into a single workflow.
* Incorporated localized agricultural knowledge for tea disease management.
* Designed recovery tracking to evaluate changes in plant health across multiple scans.

## 💻 Technologies

`Python` · `YOLOv8` · `PyTorch` · `TensorFlow` · `Keras` · `Flask` · `ChromaDB` · `SentenceTransformers` · `Llama 3.1` · `Ollama` · `PostgreSQL` · `Docker`
