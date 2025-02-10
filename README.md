# 🖼️ Image Processing Techniques: Inpainting, Steganography, and Adversarial Attacks  

This repository contains Jupyter notebooks covering three key image processing techniques: inpainting, steganography, and adversarial attacks.  

## 📌 Inpainting  
Reconstruction of missing image regions using classical methods:  
- **Navier-Stokes** – propagates information based on fluid dynamics equations, effective for smooth areas.  
- **Telea** – propagates pixel values using brightness minimization, often used for filling small gaps.  

Additionally, a **GAN-based model** has been used for more advanced image reconstruction. Details and code are available in a separate repository:  
🔗 [Link to GAN repository](https://github.com/tlatkowski/inpainting-gmcnn-keras)  

## 🔒 Steganography  
Implementation of information hiding in images using the Least Significant Bit (LSB) method.  
In this experiment, the four least significant bits of the carrier image were replaced with the four most significant bits of the embedded image.  

## ⚠️ Adversarial Attacks  
Evaluation of model robustness against adversarial attacks:  
- **Jacobian-based Saliency Map Attack (JSMA)** – manipulates selected image pixels to force misclassification.  
- **Synthesizing Robust Adversarial Examples** – generates adversarial examples that are more resistant to conventional defense techniques.  

## ⚙️ Requirements  
- Python 3.8+  
- OpenCV  
- NumPy, Matplotlib  
- Tensorflow/Keras (for adversarial attacks)  
