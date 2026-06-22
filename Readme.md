# 🛍️ AI Product Intelligence System

An AI-powered Product Intelligence System built using **CLIP**, **BLIP**, and **FAISS** for understanding products from images and text. This project was developed as part of the **Gen AI Bootcamp – Day 2 Homework Challenge**.

---

## 📌 Project Overview

This system leverages multimodal AI models to automate product understanding for e-commerce platforms. It performs:

- 📷 Product Category Prediction
- 📝 Product Description Generation
- 🔍 Similar Product Search
- 🎯 Smart Product Recommendation
- 📂 Duplicate Product Detection
- 🔄 Reverse Product Search (Text → Image)

---

## 🚀 Features

### 1. Product Category Prediction

Uses the CLIP image encoder to classify products using zero-shot learning.

### 2. Product Description Generation

Generates natural-language product descriptions using BLIP.

### 3. Similar Product Search

Uses CLIP image embeddings and FAISS vector search to retrieve visually similar products.

### 4. Smart Product Recommendation

Recommends complementary products based on the predicted product category.

Example:

**Input:** Running Shoe

**Recommendations:**

- Sports Socks
- Fitness Watch
- Water Bottle

### 5. Unique Product Catalog Creation

Detects duplicate or near-duplicate products using CLIP embeddings and cosine similarity, then groups them into a unique catalog.

### 6. Reverse Product Search

Allows users to search products using natural language.

Example:

**Query:** Blue Casual Shirt

Returns the most relevant matching product images.

---

## 🏗️ Project Architecture

```text
Product Image
      │
      ▼
Image Preprocessing
      │
      ▼
CLIP Image Encoder
      │
      ├────────► Product Category
      │
      ├────────► Image Embedding
      │
      ▼
BLIP Caption Generator
      │
      ▼
Product Description
      │
      ▼
Recommendation Engine
      │
      ▼
Duplicate Detection
      │
      ▼
Unique Product Catalog
      │
      ▼
FAISS Vector Database
      ▲
      │
Text Query
      │
      ▼
CLIP Text Encoder
      │
      ▼
Reverse Product Search
```

---

## 📂 Project Structure

```text
AI_Product_Intelligence_System/
│
├── Dataset/
├── Source_code/
│   ├── Task1_ProductUnderstanding.ipynb
│   ├── Task2_UniqueProductCatalog.ipynb
│   ├── Task3_ReverseProductSearch.ipynb
│
├── embeddings/
├── models/
├── report/
├── screenshots/
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 🛠️ Technologies Used

- Python
- PyTorch
- Transformers (Hugging Face)
- CLIP
- BLIP
- FAISS
- NumPy
- Pandas
- Scikit-learn
- Matplotlib
- Pillow
- Streamlit (Optional)

---

## 📊 Dataset

**Fashion Product Images (Small)**

https://www.kaggle.com/code/sahandakramipour/fashion-product-images-small

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/AI_Product_Intelligence_System.git
```

Move into the project folder:

```bash
cd AI_Product_Intelligence_System
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Run the Project

Launch the notebooks in Jupyter Notebook or Kaggle.

(Optional Streamlit App)

```bash
streamlit run app.py
```

---

## 📈 Future Improvements

- Real-time recommendation engine
- Multi-language product search
- Voice-based product search
- Fine-tuned CLIP model
- Large-scale vector database support

---

## 👨‍💻 Author

Chanukya Chandra

Gen AI Bootcamp – Day 2 Homework Challenge
