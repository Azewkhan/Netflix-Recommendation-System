# Netflix Movie & TV Show Recommendation System using NLP

##  Project Overview
This project builds a **personalized recommendation system** for Netflix titles using **Natural Language Processing (NLP)** techniques. By analyzing metadata like **title, cast, director, genres, and descriptions**, we developed a **content-based recommendation engine** using **TF-IDF vectorization** and **cosine similarity**.

A **Streamlit web app** was built for real-time recommendations based on user input.

## 🔥 Features
- **Content-based filtering** using TF-IDF
- **Preprocessing of Netflix metadata**
- **Cosine similarity** for title recommendations
- **Scalable & interactive** Streamlit web app
- **Performance evaluation** using Precision, Recall, and F1-score

## 📊 Dataset
We used a **publicly available Netflix dataset** containing metadata like:
- Title, Type (Movie/TV Show)
- Cast, Director, Listed Genres
- Description

### **Preprocessing Steps**
✅ Removed null values in key columns  
✅ Applied text cleaning (lowercasing, punctuation removal, whitespace normalization)  
✅ Constructed a **custom Bag-of-Words (BoW)** combining multiple columns  
✅ **Boosted genres (x3) and descriptions (x2)** for emphasis  
✅ Final dataset size after cleaning: **5,699 records**

## 🛠️ Methodology
### **Feature Engineering**
- Constructed **BoW** combining metadata fields
- Boosted **genres and descriptions** for better recommendations

### **TF-IDF Vectorization**
- Applied **TfidfVectorizer** with **bigrams** & **stopword removal**
- Created a **sparse matrix** representing word/phrase importance

### **Cosine Similarity Calculation**
- Built a **5,699 x 5,699 similarity matrix**
- Identified top recommendations based on similarity scores

### **Recommendation Engine**
- Implemented `FlixHub` class with:
  - **Title search** feature
  - **Top-N recommendations** generator

### **Deployment**
🚀 Built a **Streamlit app** with Netflix-themed UI  
🎬 Users can select a title & get real-time recommendations  

## 📊 Evaluation & Results
| Metric       | Score  |
|-------------|--------|
| Precision@10 | 0.80   |
| Recall@10    | 0.67   |
| F1 Score@10 | 0.73   |
| Accuracy (proxy) | 0.65 |

✅ The system successfully retrieves **relevant and similar titles** 🎯  
📊 Visualizations include **bar plots of metrics & content distribution**


## 📌 Future Work
🔹 Integrate **user watch history & ratings** for better recommendations  
🔹 Explore **deep learning models** (BERT, Siamese networks)  
🔹 Implement **multilingual recommendations** 🌍  

## 🏆 Team Members
- **Devesh Ojha (T00733907)** – Data Preprocessing & Feature Engineering
- **Mohd Asaf Shaikh (T00728877)** – TF-IDF Vectorization & Cosine Similarity
- **Mohammed Azeem Khan (T00736678)** – Recommendation Engine & Evaluation
- **Shaharyaar Kutchi (T00731754)** – Streamlit App & Documentation

## 📌 References
- [Scikit-learn](https://scikit-learn.org)
- [Streamlit](https://docs.streamlit.io)
- [Netflix Dataset (Kaggle)](https://www.kaggle.com/shivamb/netflix-shows)
- TF-IDF Theory – Wikipedia, Towards Data Science articles
- Cosine Similarity – Stanford NLP Notes

## 📜 License
This project is licensed under the **MIT License**. Feel free to contribute!

---
**⭐ If you found this useful, please give it a star on GitHub! ⭐**
