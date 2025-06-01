# TrendTribe 👗✨

**TrendTribe** is an AI-powered fashion recommendation system that suggests visually similar fashion items based on uploaded images. Leveraging deep learning and computer vision, it helps users discover new fashion pieces that match their style — all through an intuitive web interface built with **Streamlit**.

---

## 🚀 Features

- **📸 Upload & Recommend**: Upload an image of a fashion item to receive similar recommendations.
- **🔍 Visual Similarity Matching**: Displays the top 5 most visually similar fashion items.
- **💡 Clean UI**: Interactive and minimal interface using Streamlit.

---

## 🛠 Tech Stack

### 🔹 Frontend
- **Streamlit** – For building the web-based user interface.

### 🔹 Backend
- **Python** – Core programming language.
- **TensorFlow / Keras** – For image feature extraction using the ResNet50 model.
- **scikit-learn** – For nearest neighbor search to find similar images.
- **NumPy & Pickle** – For data manipulation and feature persistence.

---

## 📦 Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/trendtribe.git
   cd trendtribe
   ```

2. **Install the dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Add feature files:**
   Ensure the following files are present in the project directory:
   - `Image_features.pkl`
   - `filenames.pkl`

---

## ▶️ Usage

1. **Run the application:**
   ```bash
   streamlit run app.py
   ```

2. **Upload** a fashion item image via the web interface.

3. **View** the top 5 visually similar items returned by the system.

---

## 🧠 Model Overview

- **Feature Extractor**: ResNet50 pre-trained on ImageNet with the top layers removed.
- **Pooling**: A `GlobalMaxPooling2D` layer is applied to extract compact feature vectors.
- **Normalization**: L2 normalization ensures consistent feature magnitudes.
- **Similarity Search**: Euclidean distance with the `NearestNeighbors` algorithm is used to find visually similar images.

---

## 🤝 Contributing

We welcome community contributions!  
To contribute:

1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Push to the branch
5. Open a pull request

You can also report bugs or suggest features by opening issues.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙌 Acknowledgements

- Fashion dataset used to generate recommendations.
- Libraries and frameworks: TensorFlow, Keras, Streamlit, scikit-learn, NumPy, Pickle.

---


