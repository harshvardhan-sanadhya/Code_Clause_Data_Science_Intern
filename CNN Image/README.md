# 🌱 Crop Disease Detection

This project is an **end-to-end deep learning application** that detects crop diseases from images.
We trained a **Convolutional Neural Network (CNN)** model on the **Plant Disease Dataset** and deployed it using **Flask** with a simple web interface.

---

## 🚀 Features

* ✅ Image classification for multiple crop diseases
* ✅ CNN model trained with TensorFlow/Keras
* ✅ Accuracy: ~97% on training data, ~80%+ in real-world testing
* ✅ Web interface built with **HTML, CSS, Flask**
* ✅ Upload an image and get predictions with the disease name + image preview

---

## 📂 Project Structure

```
📦 crop-disease-detection
├── app.py                # Flask backend
├── crop_disease.h5       # Trained CNN model
├── model.ipynb           # Model training notebook
├── test.ipynb            # Model testing notebook
├── /static               # Static files (CSS, uploaded images)
│   └── style.css
├── /templates            # HTML templates
│   ├── index.html
│   └── result.html
└── README.md             # Project documentation
```

---

## ⚙️ Tech Stack

* **Python**
* **TensorFlow/Keras** – CNN model training
* **Flask** – Web framework
* **HTML, CSS** – Frontend UI
* **Matplotlib / NumPy** – Visualization & preprocessing

---

## 🧑‍💻 How It Works

1. Upload an image of a crop leaf using the web interface.
2. The image is preprocessed (`224x224`, normalized).
3. The trained CNN model makes predictions.
4. The result page displays the **uploaded image** along with the **predicted disease name**.

---

## 📊 Results

* **Training Accuracy:** ~97%
* **Validation Testing:** Correct on 8/10 random validation samples
* Some misclassifications happen when insects or non-leaf artifacts are present.

---


## 📌 Future Improvements

* Improve robustness with insect/noise-affected images
* Add Grad-CAM visualization to explain model predictions
* Deploy on cloud (Heroku/AWS) for public access

---

## 🎯 Conclusion

This project successfully demonstrates a **complete ML pipeline**:

* Model training
* Evaluation
* Deployment with Flask
* Working user-friendly web interface

---
