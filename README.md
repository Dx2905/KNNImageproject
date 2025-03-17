
# **Image Completion Using k-Nearest Neighbors (KNN)**  

## **📌 Project Overview**  
This project applies the **k-Nearest Neighbors (KNN) algorithm** to perform **image completion**, predicting missing pixel values based on surrounding pixels. The model estimates **continuous variables** (pixel intensities) and reconstructs images with missing data using **distance-based neighborhood estimations**.  

## **🖥️ How It Works**  
1. The input image is represented as a **2D array (matrix) of luminosity values**.  
2. Some pixels are **removed (set to missing values)**.  
3. For each missing pixel, the algorithm:  
   - Finds **K nearest neighbors** that have known luminosity values.  
   - Uses **distance metrics** (e.g., Euclidean or Manhattan) to determine closeness.  
   - Predicts the missing pixel using the **average or median of the K-nearest known values**.  
4. The completed image is reconstructed and evaluated for accuracy.  

## **🚀 Features**  
✔ Uses **k-Nearest Neighbors (KNN)** for **continuous variable regression**.  
✔ Supports **variable K-values** to fine-tune image restoration.  
✔ Demonstrates the impact of **different K-values on image quality**.  
✔ Handles **different levels of pixel loss** (50%, 75%, 90%).  
✔ Includes **visualizations** of restored images.  

## **📂 Files Included**  
- **`CS5800_Final_Project_KNN.ipynb`** - Jupyter Notebook with the complete implementation.  
- **`CS5800 K-Nearest Neighbors slide deck.pptx`** - Presentation slides explaining the project.  

## **🔧 Installation & Setup**  
### **1️⃣ Prerequisites**  
Ensure you have the following installed:  
- **Python 3.x**  
- **Jupyter Notebook**  
- **Required Libraries:**  
  ```bash
  pip install numpy pandas matplotlib scikit-learn
  ```

### **2️⃣ Running the Project**  
1. Clone this repository:  
   ```bash
   git clone https://github.com/Dx2905/Image-Completion-KNN.git
   cd Image-Completion-KNN
   ```
2. Open **Jupyter Notebook**:  
   ```bash
   jupyter notebook
   ```
3. Run **`CS5800_Final_Project_KNN.ipynb`** step by step to execute the model.  

## **📊 Experiment Results**  
| K Value | Deletion Level | Observations |  
|---------|---------------|--------------|  
| 1       | 90%          | High noise, poor results |  
| 5       | 90%          | Some structure restored, still noisy |  
| 10      | 90%          | Good balance between detail and smoothness |  
| 50      | 50%          | Too much blurring, loss of details |  

## **📌 Future Improvements**  
🔹 Try **adaptive K-values** based on pixel density.  
🔹 Implement **machine learning models** (e.g., CNNs) for comparison.  
🔹 Explore different **distance metrics** for improved accuracy.  

## **📜 License**  
This project is licensed under the **MIT License**. See the [LICENSE](https://github.com/Dx2905/CS5100-Foundation-Of-AI/blob/main/LICENSE) file for more details.  

