# Optio-Middleware 🏛️

> **"Optio acts as your backend's second-in-command. Using a 4-bit quantized LLM, it disciplines unstructured natural language inputs into validated, actionable JSON payloads."**

## 🛡️ The Concept: Why "Optio"?

In the Roman Legion, the **Centurion** commanded the cohort, but the **Optio** (his second-in-command) was responsible for keeping order, administrative details, and ensuring the soldiers stayed in line.

This project is your **Digital Optio**.
* **The User (Centurion):** Gives chaotic, unstructured natural language commands.
* **The Middleware (Optio):** Disciplines the input, enforcing strict structure.
* **The Backend (Legion):** Receives clean, validated JSON to execute actions.

## 🎯 Technical Scope

This is a specialized **Middleware AI** project, not a general-purpose chatbot. It demonstrates how to fine-tune Large Language Models (LLMs) on consumer hardware for specific format enforcement.

* **Architecture:** QLoRA (Quantized Low-Rank Adaptation)
* **Base Model:** Mistral-7B / Llama-3-8B (via Unsloth)
* **Hardware Constraint:** Optimized for **NVIDIA RTX 4060 (8GB VRAM)**
* **Serving:** FastAPI Microservice with Docker support
* **Output:** Strict JSON Schema for System-to-System integration

## 📂 Project Structure

```text
optio-middleware/
├── data/             # Synthetic datasets for format alignment
├── model/            # Unsloth training scripts & LoRA adapters
├── server/           # FastAPI application for model serving
├── client_example/   # Java client demonstrating integration
└── requirements.txt  # Dependencies (Unsloth, Torch, FastAPI)
