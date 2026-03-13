🧠 ALZ-AI: A Multi-Modal AI Suite for Alzheimer's Diagnostics & Therapeutics
Empowering Clinicians with Triple-Pillar Intelligence: Neuroimaging, Clinical Analytics, and Drug Repurposing.
ALZ-AI is an end-to-end medical intelligence platform that integrates Dual-Attention Computer Vision, Interpretable Machine Learning, and Multi-Task Molecular Binding models. This suite provides a 360-degree toolset for neurologists and pharmaceutical researchers to bridge the gap between diagnosis and treatment.
________________________________________
🚀 Key Modules & Innovation
1. Neuroimaging Engine (MRI Analysis)
•	The Architecture: Implements Multi-Instance Learning (MIL) with a Dual-Attention ResNet-18.
•	Dynamic Processing: The engine is built to handle multiple medical imaging formats.
•	DICOM/NIfTI Support: Automatically processes 3D volumes by identifying and extracting the 16 most informative anatomical slices.
•	Standard Image Support: Can process bulk .zip files containing standard image formats (JPG/PNG) for rapid screening.
•	Explainability: Features a Grad-CAM visualization suite to generate heatmaps, providing visual "Proof of Decision" for radiologists.
2. Clinical Risk Stratification
•	Logic Engine: A "glass-box" Decision Tree Classifier analyzing 31 patient variables.
•	Weighted Heuristics: Calculates a real-time Risk Level (High, Moderate, Low) by correlating cognitive scores (MMSE) with physiological and lifestyle factors.
•	Deployment: Serialized via joblib for high-speed, robust inference in clinical environments.
3. Drug Repurposing & Molecular Binding
•	Two-Stage Discovery:
•	Stage 1 (Search): Uses Cosine Similarity to match drug embeddings against a database of Alzheimer's-related GPCR protein targets.
•	Stage 2 (Validate): A Multi-Task Residual Network predicts four critical pharmacological metrics: Ki, Kd, IC50, and EC50.
•	Stability: Utilizes Residual Blocks and Layer Normalization to ensure reliable predictions in high-dimensional molecular latent spaces.
________________________________________
📂 Project Resources & Examples
To facilitate immediate testing and evaluation, the repository includes a curated examples/ directory:
•	MRI Test Suite: Contains sample .nii (NIfTI) volumes and .zip archives of 2D slices to demonstrate the model's flexibility with medical imaging standards.
•	SMILES Library: A dedicated folder containing a variety of SMILES strings (molecular representations). These can be copied directly into the Frontend Drug Discovery dashboard to observe real-time binding affinity predictions.
•	Clinical Profiles: Example JSON payloads to test the risk stratification logic for different patient demographics.
________________________________________
🛠 Tech Stack & Deployment
•	Frontend: React.js (Vite), Tailwind CSS, GSAP (Animations), Lucide Icons.
•	Backend: FastAPI (Python), Uvicorn, REST API.
•	AI/ML: PyTorch, TorchVision, Scikit-Learn, Transformers.
•	Orchestration: Docker & Docker-Compose for unified containerized deployment.
________________________________________
⚙️ Installation & Setup
Hosting via GitHub
1.	Clone the Repository:
Bash
git clone https://github.com/your-username/alz-ai.git
cd alz-ai
2.	Launch with Docker-Compose:
Bash
docker-compose up --build
3.	Access the Platform:
•	Frontend: http://localhost:3000
•	Integrated API Suite: http://localhost:8000
________________________________________
🌟 Why ALZ-AI?
ALZ-AI stands out by moving beyond simple classification. By combining Imaging, Clinical Data, and Therapeutics into a single cohesive ecosystem—and providing the raw data examples to prove it works—we provide a production-ready solution for the future of Alzheimer's care.
