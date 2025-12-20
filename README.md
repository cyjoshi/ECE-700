# NeuroXAI: Explainable Deep Learning for Multi-Modal Brain Tumor Diagnosis

- Background & Challenge: While Convolutional Neural Networks (CNNs) like ResNet have achieved radiologist-level performance in detecting brain neoplasms, their "black-box" nature creates significant trust and safety barriers in clinical settings. Clinicians cannot rely on a system that offers a diagnosis without a transparent rationale.

- Objective: This project establishes a transparent deep learning framework for brain tumor classification using a ResNet18 architecture trained on multi-modal MRI datasets (T1, T1C+, T2). The core objective is to audit the model's decision-making process using two Explainable AI (XAI) techniques: Grad-CAM and LIME.

## Key Methodologies:

- Dual-Verification: A systematic comparison between manual radiological assessment, CNN classification, and XAI visual explanations.

- Multi-Modal Synergy: The study validates a "Search and Verify" workflow, demonstrating that models use T2 sequences for high-sensitivity detection (the "Wide Net") and T1-Contrast for high-specificity confirmation (the "Validator").

## Key Findings:

- The Isointensity Trap: XAI revealed that single-modality models (T2 only) fail to detect isointense tumors like Meningiomas, necessitating multi-contrast inputs.

- Geometric Shortcuts: The model was found to use anatomical distortion (mass effect) as a shortcut in plain T1 scans, rather than analyzing tissue texture.

- Clinical Alignment: The interpretability-driven approach confirmed that the model's high precision (e.g., 100% for Glioblastoma on T1C+) is rooted in correct pathological features, bridging the gap between high-performance computing and clinical trust.

---
