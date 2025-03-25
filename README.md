# 🖼️ TP 05: Image Filtering & Convolution BY Dr Guessoum

## 🎯 Objectives  
1. Understand the concepts of **image blurring** and **filtering**.  
2. Apply **Mean** and **Gaussian** filters for smoothing images.  

---

## 📝 Steps  

### 🔹 Part 1: Blurring with Mean & Gaussian Filters  

#### 📌 1.1 Blurring "Space.bmp"  
- Apply a **Mean filter (15×15 kernel)** to **Space.bmp**.  
- Convert the blurred image to **black & white** (binarization).  
- Display the results.  

#### 📌 1.2 Blurring to Close Gaps ("GappedText.bmp")  
- Apply a **Mean filter (3×3 kernel)** to **GappedText.bmp**.  
- Convert to **black & white** to check if disconnected letters are joined.  
- Display the results.  

---

### 🔹 Part 2: Effect of Different Kernel Sizes (Joker.bmp)  

#### 📌 2.1 Mean Filter with Different Kernel Sizes  
- Apply **Mean filters** of sizes:  
  - **5×5**, **15×15**, **25×25**, **29×29** on **Joker.bmp**.  
- Analyze the effects on:  
  - **Noise points**  
  - **Letters (especially "a")**  
  - **Vertical lines in the image**  

#### 📌 2.2 Compare Mean vs. Gaussian Filter  
- Apply a **Gaussian filter (15×15 kernel)** on **Joker.bmp**.  
- Compare results with the **Mean filter (15×15)**.  

---

## 🔧 Useful OpenCV Functions  
### 📌 Mean Filter  
```python
blurred = cv2.blur(image, (kernel_size, kernel_size))
