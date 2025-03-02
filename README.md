# A Survey on IQA: Insights, Analysis, and Future Outlook

![img1](assets/Metric_Struct.jpg)

## 🔍 Introduction

Image quality assessment (IQA) represents a pivotal challenge in image-focused technologies, significantly influencing the advancement trajectory of image processing and computer vision. Recently, IQA has witnessed a notable surge in innovative research efforts, driven by the emergence of novel architectural paradigms and sophisticated computational techniques. This survey delivers an extensive analysis of contemporary IQA methodologies, organized according to their application scenarios, serving as a beneficial reference for both beginners and experienced researchers. We analyze the advantages and limitations of current approaches and suggest potential future research pathways. The survey encompasses both general and specific IQA methodologies, including conventional statistical measures, machine learning techniques, and cutting-edge deep learning models such as convolutional neural networks (CNNs) and Transformer models. The analysis within this survey highlights the necessity for distortion-specific IQA methods tailored to various application scenarios, emphasizing the significance of practicality, interpretability, and ease of implementation in future developments. Our survey aims to serve as a resource for researchers and practitioners, providing insights, related references, and continuous updates on this exciting and rapidly evolving field.

🚀Paper link: [A Survey on Image Quality Assessment: Insights, Analysis, and Future Outlook](https://arxiv.org/abs/2502.08540)

## Update Records

- 🔥 [2/12/2025] The first version of our survey has been released on arXiv.

## 📜 Table of Contents

- [📚 Image Quality Assessment Methods](#image-quality-assessment-methods)
    -  **📗  General Scene Methods**
       <details>
          <summary>📕 Statistics Methods</summary>
         
          - 📘 **HVS-Based Methods**
         
          - 📘 **Transform Domain-Based Methods**
            
          - 📘 **NSS-Based Methods**
            
       </details>
       <details>
          <summary>📕 Machine Learning-Based Methods</summary>
         
          - 📘 **Model-based Methods**
         
          - 📘 **Framework-Based Methods**
            
       </details>
    -  **📗  Specific Scene Methods**
          - 📕 **Medical IQA**
         
          - 📕 **IQA for Dehazing Algorithms**
     
          - 📕 **Portrait Quality Assessment**
     
          - 📕 **Specific Distortion**

- [🌐 More Comprehensive Summarization](#-more-comprehensive-summarization)
- [👨‍👨‍👧‍👦 Maintainers](#-maintainers)
- [📚 Citation](#-citation)
- [💪 How to Contribute](#-how-to-contribute)
- [🫡 Acknowledgement](#-acknowledgement)
- [📧 Contact Us](#-contact-us)

## 📚 Image Quality Assessment Methods

IQA methods can be categorized based on their dependency on reference images:

- **Full-Reference IQA (FR-IQA)**: Requires a pristine reference image for comparison.
- **Reduced-Reference IQA (RR-IQA)**: Uses partial reference information for assessment.
- **No-Reference IQA (NR-IQA)**: Assesses image quality without any reference image.

## 🛠 Key Techniques and Methodologies

### 📊 Traditional IQA Metrics
- Peak Signal-to-Noise Ratio (PSNR)
- Structural Similarity Index (SSIM)
- Visual Information Fidelity (VIF)

### 🤖 Learning-Based IQA
- Convolutional Neural Network (CNN)-based models
- Transformer-based IQA models
- No-reference deep learning methods

### 🏗 Hybrid Approaches
- Combining statistical and deep learning-based techniques
- Multi-scale feature extraction for perceptual quality assessment

## 🚀 Applications

IQA methods are widely used in various domains, including but not limited to:

- **Image Compression and Enhancement**
- **Medical Imaging Quality Assessment**
- **Autonomous Driving and Surveillance**
- **Multimedia Streaming and Transmission**
- **Photo Editing and Aesthetic Assessment**

## ⚠ Challenges and Open Problems

Despite advancements, IQA faces several challenges:

- **Subjective vs. Objective Quality Discrepancy**: Bridging the gap between human perception and objective metrics.
- **Generalization and Robustness**: Ensuring model performance across diverse datasets.
- **Real-Time Processing**: Reducing computational overhead for real-time applications.
- **Interpretable and Explainable IQA**: Enhancing transparency in deep learning-based IQA models.

## 🔭 Future Directions

- **Self-Supervised Learning for IQA**: Reducing reliance on labeled datasets.
- **Cross-Domain Generalization**: Improving robustness across different image types.
- **Efficient and Lightweight Models**: Developing IQA methods for resource-constrained devices.
- **Benchmarking and Standardization**: Establishing unified evaluation metrics and datasets.

## 📖 References

A comprehensive list of references is maintained in the [`references.bib`](./references.bib) file.
