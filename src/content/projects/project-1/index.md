---

title: "Lab Report Analyzer"

description: "LLM-powered blood report analyzer."

date: "Sep 2026"

demoURL: "https://github.com/visharaaa/lab-report-analyzer"

repoURL: "https://github.com/visharaaa/lab-report-analyzer"

---

![Lab Report Analyzer](/lab-report-analyzer.png)

Lab Report Analyzer is an AI-powered application designed to convert blood test reports into structured results and explain them in clear, easy-to-understand language.

The system focuses on CBC, HbA1c and blood glucose results, combining structured data extraction, result normalization, Retrieval-Augmented Generation (RAG), and an LLM to provide contextual explanations while keeping safety and uncertainty in mind.

## 📋 Features

* Blood report text extraction
* Structured laboratory result parsing
* Result normalization and standardization
* CBC analysis
* HbA1c analysis
* Blood glucose analysis
* Reference range interpretation
* Retrieval-Augmented Generation (RAG)
* Medical knowledge base
* Plain-language explanations
* Confidence-aware processing
* Safety-focused response handling
* Pydantic data validation
* Automated testing with pytest

## 🤖 AI & RAG

The application uses a Retrieval-Augmented Generation pipeline to provide explanations based on a curated knowledge base rather than relying entirely on the language model's internal knowledge.

Relevant information is retrieved based on the extracted laboratory results and passed to the LLM as contextual information for generating the final explanation.

The current knowledge base focuses on:

* **CBC:** Complete Blood Count parameters and common interpretations
* **HbA1c:** Long-term blood glucose measurement and reference ranges
* **Glucose:** Blood glucose measurements and contextual interpretation

## 🔄 Processing Pipeline

1. Extract laboratory results from a blood report.
2. Parse values, units and reference ranges.
3. Normalize test names into standardized representations.
4. Validate the structured results using Pydantic models.
5. Retrieve relevant information from the medical knowledge base.
6. Provide the retrieved context to the language model.
7. Generate a plain-language explanation.
8. Apply safety-focused handling before presenting the response.

## 🏗️ Architecture

The project is organized into modular components for extraction, normalization, retrieval, LLM processing and safety handling.

* **Extraction:** Converts report text into structured laboratory results.
* **Normalization:** Standardizes test names, units and values.
* **RAG:** Retrieves relevant information from the knowledge base.
* **LLM:** Generates contextua

