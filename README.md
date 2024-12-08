### Machine Learning for Serabutin App 🚀🤖  

This folder contains resources, models, and scripts for the **Machine Learning (ML) components** in the Serabutin app. The app focuses on providing efficient and user-friendly solutions for managing various tasks, like finding nearby helpers for odd jobs, with a strong emphasis on **localization, safety, and ethical compliance**.

---

### Features  

#### 🧑‍🤝‍🧑 Face Verification Using Landmarks 🌟  
A robust face verification system designed to ensure safety and user identity in the Serabutin app.  

**Key Highlights**:  
- **Face Detection**: Detects faces using Haar Cascade classifiers.  
- **Face Alignment**: Aligns detected faces for consistency using landmarks.  
- **Verification**: Compares normalized facial landmarks using Euclidean distance to determine matches.  

**Workflow**:  
1. Detect faces in two images.  
2. Align faces based on landmarks.  
3. Normalize and compare landmarks.  
4. Decide match/no match based on distance threshold.  

**Future Enhancements**:  
- Transition to advanced face detection (e.g., MTCNN).  
- Integrate deep learning for precise verification.  

---

#### 🤖 Illegal Job Post Filtering Using NLP  
An NLP-based system to automatically detect and filter illegal or inappropriate job postings, ensuring platform compliance with ethical and legal standards.  

**Key Highlights**:  
- Utilizes a **Bidirectional LSTM model** for text classification.  
- Flags prohibited content with high accuracy to maintain platform integrity.  

**Workflow**:  
1. Preprocess job descriptions into embeddings.  
2. Use bidirectional LSTM layers for contextual feature extraction.  
3. Apply dense layers for binary classification (Legal/Illegal).  

**Future Enhancements**:  
- Dynamic model updates for evolving legal requirements.  
- Expand dataset diversity to improve robustness.  

---

### Requirements  
- **Python 3.8+**  
- **ML Libraries**: TensorFlow, NumPy, Pandas, Scikit-learn  
- **CV Libraries**: OpenCV  

**Install**:  
```bash  
pip install -r requirements.txt  
```  

---

### Roadmap  
- Integrate both ML modules into the Serabutin app for seamless use.  
- Enhance safety and user experience with localization and real-time validation.  
- Implement dynamic model updates for adaptability and precision.  

---  
Contributions and suggestions are welcome! 🌟
