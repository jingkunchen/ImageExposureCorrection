# Balancing Light and Shadow: A Benchmark for Multi-Modal Exposure Correction via Frequency–Phase Driven RGB-IR Integration
---

## Abstract

Capturing high-quality images under dynamic and extreme illumination conditions remains a challenging problem. Conventional imaging methods relying solely on RGB or infrared (IR) modalities often fail when faced with deep shadows and harsh highlights: RGB images suffer from noise and loss of detail in low-light regions, while IR images lack the fine texture and color cues required for high-fidelity reconstruction. In our approach, we introduce a multi-modal framework that leverages frequency-domain analysis to decompose RGB and IR images into amplitude and phase components. By exchanging IR amplitude with RGB phase, our method reduces reconstruction errors and enhances image quality. The framework is built upon a dual-branch encoder–decoder architecture featuring a hierarchical Spectral–Phase Fusion Pyramid and a BiFusion Attention Transformer for robust cross-modal integration. Extensive experiments on a newly established HDRT dataset demonstrate significant improvements across image quality metrics and downstream tasks, including classification, segmentation, and object detection.

### Dataset Details

- **HDRT Dataset Overview:**  
  The HDRT dataset is designed to support multi-modal exposure correction research. It comprises 10,000 scenes, with each scene providing four images (totaling 40,000 images):
  - **Low-Exposure (LE) RGB Image:** Severely underexposed image.
  - **High-Exposure (HE) RGB Image:** Severely overexposed image.
  - **Normal-Exposure (Reference) RGB Image:** Properly exposed image serving as the ground truth.
  - **Infrared (IR) Image:** Captures robust illumination cues under extreme conditions.

- **Access:**  
  The dataset is publicly accessible at [Hugging Face HDRTDataset](https://huggingface.co/datasets/jingchao-peng/HDRTDataset).

---

## Repository Structure

- **/manuscript:**  
  Contains the draft manuscript (PDF format) with full details on our theoretical background, network design, experiments, and ablation studies.

- **/code:**  
  Source code for the proposed framework, including scripts for training, evaluation, and inference.

- **/data:**  
  Documentation and scripts to assist with downloading and preparing the HDRT dataset.

- **/supplementary:**  
  Additional experimental details and extended results supporting the main paper.

---

## Usage

### Getting Started

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/jingkunchen/BLS.git
   cd BLS
