# U-Net-Semantic-Segmentation
**U-Net-Based Semantic Segmentation for Brain Tumor Diagnosis**

## Project Level : High-Intermediate 
*You may find the report of the project under the name "U-Net-Based Semantic Segmentation for Brain Tumor Diagnosis-Solouki.PDF"*

---

###  **Project Highlights**
- Semantic segmentation of brain MRI images using an enhanced U-Net architecture  
- Based on the 2022 paper: *Brain Tumor Segmentation using Enhanced U-Net Model with Empirical Analysis*  
- Trained on LGG segmentation dataset from The Cancer Imaging Archive (TCIA)  
- Comprehensive preprocessing including resizing, normalization, and augmentation  
- Trained & Evaluated using IoU and Dice Coefficient metrics  

---

###  **Project Goal**  
To segment brain tumors in MRI images using a modified U-Net deep learning model, aiming to assist in precise localization of tumor regions for improved diagnosis and medical analysis.

---

###  **Project Description**  
The project addresses semantic segmentation of brain tumors using MRI scans from the **LGG (Lower Grade Glioma)** dataset. This dataset contains manually labeled FLAIR (Fluid-Attenuated Inversion Recovery) abnormality masks for 110 patients. The data was obtained from **The Cancer Genome Atlas (TCGA)** via **The Cancer Imaging Archive (TCIA)** and accessed through Kaggle using an access token.

Images were resized to **128×128** pixels as per the baseline paper, and **MinMax Scaling** was applied for normalization. The dataset was split into training, validation, and testing sets with an 80%-10%-10% ratio.

The segmentation model used is a modified version of the **U-Net** architecture, originally introduced in 2015 for biomedical image segmentation. This model includes improvements proposed in the 2022 study, focusing on enhanced empirical performance in brain tumor detection.

---

### **Language and Libraries Used**
- **Language**: Python  
- **Libraries**:  
  - NumPy  
  - TensorFlow / Keras  
  - OpenCV  
  - Matplotlib  
  - scikit-learn  

---

###  **Methods and Models**
1. **Image Preprocessing**  
   - Resized all MRI scans to 128×128 pixels  
   - Applied **MinMax Scaling** for normalization  

2. **Dataset Splitting**  
   - 80% Training  
   - 10% Validation  
   - 10% Testing  

3. **Data Augmentation Techniques**  
   - Rotation  
   - Flipping  
   - Shifting  
   - Cropping and Zooming  
   - Cropping with Padding  
   - Shearing  
   - Adding Noise  
   - Gaussian Filtering  

4. **Model Architecture**  
   - Enhanced U-Net based on the 2022 paper  
   - Convolutional layers with downsampling and upsampling paths  
   - Skip connections to retain spatial features  
   - Tailored for semantic segmentation tasks in medical imaging  

5. **Training and Evaluation**  
   - Evaluation Metrics:  
     - **IoU (Intersection over Union)**  
     - **Dice Coefficient**  

Model Perfomance on Test Data:
PERFORMANCE ON VALIDATION DATA	METRIC
0.0272	Loss
0.9936	Accuracy
0.7930	dice coef
0.7766	jacard (IoU)

![image](https://github.com/user-attachments/assets/0ffadead-b60a-4bc0-a669-b6a3556b64de)
![image](https://github.com/user-attachments/assets/a7b4d2be-a626-4b50-bd52-382958effdc0)


---
