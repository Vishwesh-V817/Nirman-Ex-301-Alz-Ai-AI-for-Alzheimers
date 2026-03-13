# 🧠 ALZ-AI: Multi-Modal Intelligence Suite
### *Diagnostics & Therapeutics for Alzheimer’s Disease*

[![FastAPI](https://img.shields.io/badge/Backend-FastAPI-009688?style=flat-square&logo=fastapi)](https://fastapi.tiangolo.com/)
[![React](https://img.shields.io/badge/Frontend-React-61DAFB?style=flat-square&logo=react)](https://reactjs.org/)
[![PyTorch](https://img.shields.io/badge/AI-PyTorch-EE4C2C?style=flat-square&logo=pytorch)](https://pytorch.org/)
[![Docker](https://img.shields.io/badge/Deployment-Docker-2496ED?style=flat-square&logo=docker)](https://www.docker.com/)

**ALZ-AI** is an end-to-end medical intelligence platform that integrates Dual-Attention Computer Vision, Interpretable Machine Learning, and Multi-Task Molecular Binding models. It provides a 360-degree toolset for neurologists and pharmaceutical researchers to bridge the gap between diagnosis and treatment.

---

## 🚀 Key Modules & Innovation

### 1. Neuroimaging Engine (MRI Analysis) 🖼️
* **The Architecture:** Implements **Multi-Instance Learning (MIL)** with a **Dual-Attention ResNet-18**.
* **DICOM/NIfTI Support:** Automatically processes 3D volumes by identifying and extracting the **16 most informative anatomical slices**.
* **Standard Image Support:** Bulk `.zip` processing for standard formats (JPG/PNG).
* **Explainability:** Features a **Grad-CAM** visualization suite to generate heatmaps, providing visual "Proof of Decision" for radiologists.

### 2. Clinical Risk Stratification 📊
* **Logic Engine:** A "glass-box" **Decision Tree Classifier** analyzing 31 patient variables.
* **Weighted Heuristics:** Calculates real-time Risk Levels (High, Moderate, Low) by correlating **MMSE scores** with physiological and lifestyle factors.
* **Deployment:** Serialized via `joblib` for high-speed, robust inference.

### 3. Drug Repurposing & Molecular Binding 💊
* **Two-Stage Discovery:**
    * **Stage 1 (Search):** Uses Cosine Similarity to match drug embeddings against Alzheimer's-related GPCR protein targets.
    * **Stage 2 (Validate):** A **Multi-Task Residual Network** predicts four critical pharmacological metrics: $K_i$, $K_d$, $IC_{50}$, and $EC_{50}$.
* **Stability:** Utilizes Residual Blocks and Layer Normalization to ensure reliable predictions in high-dimensional molecular latent spaces.

---

## 🛠️ Tech Stack & Deployment

| Layer | Technologies |
| :--- | :--- |
| **Frontend** | React.js (Vite), Tailwind CSS, GSAP, Lucide Icons |
| **Backend** | FastAPI (Python), Uvicorn, REST API |
| **AI/ML** | PyTorch, TorchVision, Scikit-Learn, Transformers |
| **Orchestration** | Docker & Docker-Compose |

---

## 📂 Project Resources & Examples
The repository includes a curated `examples/` directory for immediate evaluation:

* **MRI Test Suite:** Sample `.nii` volumes and `.zip` archives of 2D slices.
* **SMILES Library:** Molecular representations for the Frontend Drug Discovery dashboard.
* **Clinical Profiles:** Example JSON payloads to test risk stratification logic.

---

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone [https://github.com/your-username/alz-ai.git](https://github.com/your-username/alz-ai.git)
cd alz-ai

. Launch with Docker-Compose
Bash
docker-compose up --build
3. Access the Platform
Frontend: http://localhost:3000

Integrated API Suite: http://localhost:8000/docs

🌟 Why ALZ-AI?
ALZ-AI moves beyond simple classification. By combining Imaging, Clinical Data, and Therapeutics into a single cohesive ecosystem, it provides a production-ready solution for the future of Alzheimer's care.
