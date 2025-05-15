
# 🖼️ **Digital Watermarking using DCT: Manual vs Built-in Approach** 

**Author:** [Dipanshu Modi](https://github.com/dipanshumodi31) 
**Skills:** Python, Pandas, Matplotlib, OpenCV, NumPy, Image Processing, DCT, PSNR/SSIM, Visualization 
---

## 🚀 **Project Overview**  
This project explores **digital image watermarking using the Discrete Cosine Transform (DCT)**, implementing both a **manual** and **OpenCV built-in** approach to embed and evaluate watermark robustness.

📌 **Project Highlights:**  
✅ Manual 2D DCT and IDCT implementation  
✅ Watermark embedding via DCT coefficient modulation  
✅ Quality assessment using PSNR, SSIM, and MSE  
✅ Visual and statistical comparison of built-in vs manual methods  

---

## 🎯 **Key Objectives**  
✔ Apply 2D DCT to grayscale images manually and with OpenCV  
✔ Embed watermark data (binary form of string) into DCT coefficients  
✔ Reconstruct images using IDCT  
✔ Evaluate and compare results using image quality metrics  
✔ Visualize differences and assess effectiveness of both approaches  

---

## 🧠 **Core Concepts Used**  
- **DCT (Discrete Cosine Transform):** Converts spatial image data into frequency domain
- **Watermarking:** Embedding hidden binary data in transform domain  
- **Metrics:**  
  - PSNR: Measures signal fidelity  
  - SSIM: Measures perceived image quality  
  - MSE: Measures reconstruction error  

---

## 🔍 **Workflow Summary**  

### **1️⃣ Import and Visualize the Image**  
- Load the image in both RGB and Grayscale formats  
- Display side-by-side using `matplotlib`

### **2️⃣ Apply Built-in OpenCV DCT**  
- Use `cv2.dct()` to get frequency representation  
- Embed watermark data (from the string `"V7Shinobi"`) by slightly modifying DCT coefficients  
- Save and visualize the result  
- Calculate PSNR and SSIM

### **3️⃣ Manual DCT & Watermark Embedding**  
- Manually construct DCT transform matrices  
- Apply matrix multiplication to perform 2D DCT  
- Embed watermark into DCT domain  
- Calculate PSNR, SSIM

### **4️⃣ Compare Built-in vs Manual Methods**  
- Display original, built-in watermarked, and manually watermarked images  
- Compare all metrics: PSNR, SSIM, MSE  
- Visualize difference images (pixel-wise absolute error)

---

## 📊 **Performance Metrics Summary**

| Metric            | Built-in Method | Manual Method |
|-------------------|------------------|----------------|
| PSNR              | ✅ Calculated    | ✅ Calculated  |
| SSIM              | ✅ Calculated    | ✅ Calculated  |
| MSE               | ✅ Calculated    | ✅ Calculated  |

---

## 🖼️ **Visual Results**  

### DCT Domain Visualization  
- Log-scaled DCT representation before watermarking  

### Watermarked Outputs  
- Built-in and manual methods displayed side-by-side

### Difference Analysis  
- Pixel-wise error between:  
  - Original vs Built-in  
  - Original vs Manual

---

## 🛠 **How to Run This Project**  

1️⃣ Clone the repository  
```bash
git clone https://github.com/https://github.com/dipanshumodi31/DCT-Based-Digital-Watermarking-A-Comparative-Study
```

2️⃣ Install required Python packages  
```bash
pip install numpy opencv-python matplotlib scikit-image pandas pillow
```

3️⃣ Run the Jupyter Notebook  
```bash
jupyter notebook dct_image_processing.ipynb
```

---

## 💡 **Future Enhancements**  
- Encrypt watermark using cryptographic hash  
- Add robustness tests (e.g. noise, compression)  
- Expand to color image watermarking  
- Try other transforms like DWT or FFT

---
