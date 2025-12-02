# Xception: Paper Review and Implementation

This repository contains my review, presentation materials, summary report, and practical implementations of the architecture introduced in the research paper:

**Xception: Deep Learning with Depthwise Separable Convolutions**  
*François Chollet, Google Inc. (2017)*  
📄 Paper Link: https://arxiv.org/abs/1610.02357

---

## 📌 Repository Content

- **/presentation** – Slides explaining the key ideas of Xception, depthwise separable convolutions, and experimental results.
- **/report** – A written summary and analysis of the original paper.
- **/notebooks** – Jupyter notebooks implementing Xception or simplified versions.
- **/src** – Clean-code implementation of modules such as depthwise convolution, pointwise convolution, and Xception blocks.
- **/experiments** – Training logs, comparison charts, and ablation studies.

---

## 🧠 What is Xception?

Xception is a convolutional neural network architecture proposed as an improvement over Inception.  
It replaces Inception modules with **depthwise separable convolutions**, leading to:

- Better parameter efficiency  
- Lower computational cost  
- Improved accuracy on ImageNet  

The main idea is to decouple spatial filtering and channel mixing:

- **Depthwise Convolution:** A separate convolution per channel  
- **Pointwise Convolution (1×1):** Combines channel information  

This separation approximates Inception modules but in a more elegant, scalable way.

---

## 🚀 Implementation

The repository includes a minimal PyTorch/TensorFlow implementation showing:

- Depthwise separable convolution layer  
- Xception entry, middle, and exit flow blocks  
- Training script with dataset loader  
- Model summary and profiling

---

## 🧪 Experiments

Example experiments included:

- Comparing standard conv vs depthwise separable conv  
- Parameter count analysis  
- Training Xception on a small dataset  
- Visualizations of feature maps  

---

## 📚 Reference

If you use this repository for academic purposes, please cite the original paper:

Chollet, F. (2017). *Xception: Deep Learning with Depthwise Separable Convolutions.*  
arXiv:1610.02357  
https://arxiv.org/abs/1610.02357

---

## 📝 Notes

This repository is intended for educational, experimental, and presentation purposes.  
Feedback and contributions are welcome!
