# GigaSistêmica: Advancing Systemic Health Diagnostics through AI

## Overview
GigaSistêmica is a collaborative initiative between GigaCandanga and the University of Brasília (UnB), dedicated to leveraging artificial intelligence (AI) to advance diagnostic and predictive capabilities for systemic health conditions. This project focuses on integrating dental imaging, radiomic analysis, and specialized language models to develop tools for early detection and efficient healthcare delivery. As part of our commitment to open science, this repository provides a central point for tracking our research progress and associated resources.

### Projects and Publications
Below is an overview of completed and ongoing projects under the GigaSistêmica initiative. The repository will be updated as new milestones are achieved.

---

### 1. GigaXReport: A Multimodal Diagnostic Framework with Specialized Language Models (SLMs)
- **Description:**  
  GigaXReport is a Flask-based web application that unifies three advanced AI pipelines for medical imaging analysis:
  1. **Osteoporosis Detection:** Uses an EfficientNet-B7 CNN (pretrained on mandibular cortical morphology) with Grad-CAM saliency maps to classify panoramic radiographs into “Healthy” vs. “Osteoporotic” categories.  
  2. **Carotid Atheroma Analysis:** Applies a FastViT classifier to screen for atheroma presence, a Faster R-CNN ONNX model for localization, and a DC-UNet segmentation network to precisely delineate calcifications.  
  3. **Multimodal Reporting (MedGemma):** Leverages Google’s MedGemma Small Language Model (SLM), a vision-language model, to generate detailed radiological reports in English or Portuguese, embedding the AI outputs verbatim under sections such as “Bone Health” and “Atheroma Diagnosis.”  
  The app produces an interactive combined visualization (original image, Grad-CAM overlay, detection/segmentation results) and compiles a professional PDF report with embedded figures and formatted text.

- **Repository:**  
  [GitHub: BrunoScholles98/GigaXReport-A-Multimodal-Diagnostic-Framework-with-Specialized-Language-Models-SLMs](https://github.com/BrunoScholles98/GigaXReport-A-Multimodal-Diagnostic-Framework-with-Specialized-Language-Models-SLMs/tree/main)

![](https://raw.githubusercontent.com/BrunoScholles98/GigaXReport-A-Multimodal-Diagnostic-Framework-with-Specialized-Language-Models-SLMs/refs/heads/main/static/MainPage_Example.png)

---

### 2. Osteoporosis Screening with Panoramic Radiographs
- **Description:**  
  An AI-based approach to identify signs of osteoporosis using dental panoramic radiographs (PR). EfficientNet-based convolutional neural networks (CNNs) were trained on PR images to classify mandibular cortical morphology into “Healthy” (C1) and “Osteoporotic” (C3) categories. Validation was performed against Dual-energy X-ray Absorptiometry (DXA) results. Grad-CAM visualizations highlight critical regions such as the mandibular cortex.

- **Publication:**  
  Dias, B. S. S., Querrer, R., Figueiredo, P. T., Leite, A. F., de Melo, N. S., Costa, L. R., Caetano, M. F., & Farias, M. C. Q. (2025). *Osteoporosis screening: Leveraging EfficientNet with complete and cropped facial panoramic radiography imaging*. **Biomedical Signal Processing and Control**, *100*, 107031. [https://doi.org/10.1016/j.bspc.2024.107031](https://doi.org/10.1016/j.bspc.2024.107031).

- **Repository:**  
  [GitHub: BrunoScholles98/Deep-Learning-for-Bone-Health-Classification-through-X-ray-Imaging](https://github.com/BrunoScholles98/Deep-Learning-for-Bone-Health-Classification-through-X-ray-Imaging)

![Osteoporosis Screening](https://raw.githubusercontent.com/GIGASISTEMICA/GigaSistemica-Advancing-Systemic-Health-Diagnostics-through-AI/refs/heads/main/static/gitrepo_home_osteo.png)

---

### 3. Detection and Segmentation of Carotid Atheroma Calcification
- **Description:**  
  Hybrid deep learning model combining an attention-augmented classification head with a UNet segmentation backbone to detect and segment carotid atheroma calcifications (CACs) in panoramic radiographs. Provides a two-step automated pipeline for opportunistic screening in dental settings.

- **Status:** Under review at *IEEE Journal of Biomedical and Health Informatics (JBHI)*.

- **Publication:**  
  Correia, I. B. M. C., Ferreira, M. V. S., Chini, C. F., Dias, B. S. S., Costa, L. R., Caetano, M. F., Leite, A. F., de Melo, N. S., & Farias, M. C. Q. (2024). *Detection and segmentation of carotid atheroma calcification in dental panoramic radiographs using a hybrid deep learning model*. Submitted to **IEEE Journal of Biomedical and Health Informatics**.

- **Repository:**  
  [GitHub: igorbispo99/GigaSistemica-Atheroma](https://github.com/igorbispo99/GigaSistemica-Atheroma/tree/main)

![Atheroma Segmentation](https://raw.githubusercontent.com/GIGASISTEMICA/GigaSistemica-Advancing-Systemic-Health-Diagnostics-through-AI/refs/heads/main/static/gitrepo_home_ath.png)

---

### 4. Radiomic Signature Based on Cone-Beam CT for Osteoporosis Evaluation
- **Description:**  
  Development of a radiomic signature from cone-beam computed tomography (CBCT) images to evaluate osteoporosis by analyzing mandibular radiomorphometric indices.

- **Publication:**  
  Master’s thesis abstract available: [UnB SIGAA](https://sigaa.unb.br/sigaa/public/programa/noticias_desc.jsf?lc=en_US&id=907&noticia=8652785).

- **Repository:** Under development.

---

### 5. Gunshot Wounds Classification with Deep Learning (Collaboration)
- **Description:**  
  Deep learning models applied to forensic analysis of gunshot wounds: classifying entry vs. exit wounds and estimating medico-legal shooting distance (MLSD) from digital photographs. Developed in collaboration with GigaSistêmica researchers.

- **Publication:**  
  Lira, R. Q. N., Sousa, L. G. M., Pinho, M. L. M., Lima, R. C. P. S. A., Freitas, P. G., Dias, B. S. S., Souza, A. C. B., & Leite, A. F. (2024). *Deep learning-based human gunshot wounds classification*. **International Journal of Legal Medicine**, Published 6 November 2024. [https://doi.org/10.1007/s00414-024-03355-4](https://doi.org/10.1007/s00414-024-03355-4).

- **Repository:**  
  [GitLab: leguwoi](https://gitlab.com/lisa-unb/leguwoi)

---

### Data Request
If you wish to access any of the datasets associated with the projects described in this repository, please get in touch as detailed in the **Contact** section. All requests will be evaluated to ensure compliance with ethical standards and data-sharing agreements.

---

### Future Directions
The GigaSistêmica project continues to evolve, with current efforts focused on:
- **Fine-tuning a Large Language Model (LLM):** Development of a multimodal system that integrates imaging and text-based data for comprehensive systemic health analysis. This project is in its early stages.
- **Enhanced Interoperability:** Integrating developed models into a unified diagnostic pipeline for public health applications.

---

### Contact
For further inquiries or collaboration opportunities, please contact any of the coordinators listed below, or reach out to me directly via email: [brunoscholles98@gmail.com](mailto:brunoscholles98@gmail.com) or via WhatsApp at +351 913 686 499.

---

### Coordinators
Our academic and research leaders include:
- [Mylène C. Q. Farias](https://userweb.cs.txstate.edu/~mylene/)
- [André Ferreira Leite](http://lattes.cnpq.br/7275660736054053)
- [Nilce Santos de Melo](http://lattes.cnpq.br/4611919012909264)
- [Marco F. Caetano](https://cic.unb.br/professores/94-mfcaetano)

---

This repository reflects our ongoing commitment to transparency and collaboration in the scientific community. Contributions and feedback are always welcome.
