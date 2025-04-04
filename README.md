# PneuNet
# 🏥 Chest X-ray Pneumonia Detection using Autoencoder & CNN  

This project implements a **Convolutional Autoencoder** to learn meaningful latent representations from chest X-ray images. A CNN classifier is then trained on the latent features to detect pneumonia.  

---

## 📂 Dataset  

The dataset consists of chest X-ray images categorized into **training, validation, and test** sets.  


---

## 🚀 Model Architecture  

### **1. Convolutional Autoencoder**  
- **Encoder:**  
  - 3 Convolutional layers (ReLU activation)  
  - Downsamples the input image to a lower-dimensional latent space  

- **Decoder:**  
  - 3 Transposed Convolutional layers (ReLU & Sigmoid)  
  - Reconstructs the input from the latent space  

### **2. CNN Classifier (on Latent Features)**  
- Extracts the encoded features from the autoencoder  
- Passes them through CNN layers followed by a fully connected layer  
- Outputs a single value (binary classification for pneumonia detection)  

---




