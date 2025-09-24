# Blood Cancer Classification

A machine learning / deep learning project to classify types of leukemia (Benign, Early Pre-B, Pre-B, Pro-B) from medical images using feature extraction + dimensionality reduction + classification models.

---

## 🧾 Overview

- Developed a **multiclass leukemia classifier** to distinguish among \[Benign, Early Pre-B, Pre-B, Pro-B\] subtypes  
- Built a 3-step image analysis pipeline using **ResNet-50** for feature extraction  
- Performed dimensionality reduction using **PCA + Particle Swarm Optimization (PSO)**, reducing feature space by ~80%  
- Trained and evaluated models on 5,000+ images, achieving ~93% accuracy, 0.91 F1-score, and 0.89 recall  
- Created an interactive **Streamlit dashboard** for visualizing results and live demo deployment  

---

## 📁 Repository Structure

Blood-Cancer-Classification/
│
├── Dataset/ # Original / processed image dataset
├── features.npy # Extracted features from ResNet
├── pso_features.npy # Features after PCA + PSO
├── ml-project(2).ipynb # Jupyter notebook with modeling & evaluation
├── README.md # This file
├── (other scripts / modules) # Data processing, model training, utility scripts
└── ...

yaml
Copy code

---

## 🛠 Installation & Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/Daddy-28/Blood-Cancer-Classification.git
   cd Blood-Cancer-Classification
Install dependencies (preferably in a virtual environment):

bash
Copy code
pip install -r requirements.txt
Prepare data paths and set configurations (e.g. in config file or environment variables).

Run the notebook or scripts to train, evaluate, and visualize results.

🚀 Usage
Use the notebook ml-project(2).ipynb to walk through data loading, feature extraction, dimensionality reduction, model training, and evaluation.

After training, launch the Streamlit dashboard (if included) to see classification results, confusion matrices, and per-sample predictions.

You can swap in different classifiers or tweak PSO/PCA parameters to improve accuracy or generalization.

📊 Results & Metrics
~93% accuracy on the test set

0.91 F1-score

0.89 recall

These results confirm the model’s strong ability to distinguish among the leukemia subtypes with limited error.

🔍 Potential Improvements & Extensions
Experiment with other backbone models (e.g. EfficientNet, DenseNet) for feature extraction

Use alternative dimensionality reduction or feature selection methods

Incorporate data augmentation or transfer learning to improve robustness

Deploy as a web app or REST API for real-world clinical use

Add explainability / interpretability tools (e.g. Grad-CAM, SHAP) to visualize model decisions


For questions or collaboration, feel free to open an issue or reach out via GitHub.

pgsql
Copy code
