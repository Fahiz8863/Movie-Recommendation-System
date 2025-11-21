# Movie-Recommendation-System
Movie Recommendation System using content-based filtering. It analyzes movie metadata like genres, cast, director, and keywords to suggest similar movies using text vectorization and cosine similarity. Demonstrates NLP, feature engineering, and machine learning skills.

# 🎬 Movie Recommendation System  
A Content-Based Filtering Project Using Python

## 📌 Project Overview  
This project implements a **Content-Based Movie Recommendation System** that suggests movies similar to a selected movie by analyzing descriptive features such as **genres, keywords, cast, director, and storyline overview**.  

The project demonstrates key concepts in **data preprocessing, feature engineering, text vectorization, and similarity computation**, which are widely used in modern recommendation engines.

---

## 🚀 Key Features  
- Content-based recommendation using metadata  
- Text cleaning and preprocessing  
- Creation of a combined "tags" feature  
- Vectorization using **CountVectorizer**  
- Similarity calculation using **cosine similarity**  
- Function to recommend the **top 5 similar movies**

---

## 📂 Dataset  
The dataset contains **4,803 movies** with details such as:
- Title  
- Genres  
- Keywords  
- Cast  
- Director  
- Tagline  
- Overview  

For building the recommendation model, the following five features were selected:
- **genres**
- **keywords**
- **tagline**
- **cast**
- **director**

---

## 🧠 Methodology  

### **1. Data Loading**
The dataset was imported and explored to understand the number of entries and available metadata.

### **2. Feature Selection**
Five important textual features were selected because they contribute most to describing movie content.

### **3. Data Cleaning**
Missing values in the selected columns were handled by filling empty strings and standardizing the text.

### **4. Feature Engineering**
A new column called **tags** was created by combining important metadata.  
This provides a unified textual representation of each movie.

### **5. Text Vectorization**
The tags column was converted into numerical form using **CountVectorizer**, generating a 2000-dimensional feature vector for each movie.

### **6. Similarity Computation**
A **cosine similarity matrix** was calculated to measure the closeness between movies based on their vectorized tags.

### **7. Recommendation Function**
A function was created to:
- Accept a movie name  
- Retrieve its index  
- Find similarity scores  
- Recommend the **top 5 most similar movies**

---

## 📊 Example Output  

### **Input Movie:** *Avatar*

### **Recommended Movies:**  
- John Carter  
- Guardians of the Galaxy  
- Star Trek Beyond  
- Jupiter Ascending  
- The Helix…

These results show movies that share similar genres, themes, and metadata.

---

## 🛠️ Technologies Used  
- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Jupyter Notebook  

---

## 📈 Applications  
- Movie streaming platforms  
- Content discovery systems  
- Entertainment analytics  
- Personalized recommendation engines  

---

## 🔮 Future Enhancements  
- Integrate TMDB API for real-time movie data  
- Add Collaborative Filtering  
- Use TF-IDF / Word2Vec embeddings  
- Convert into a web app using Streamlit or Flask  

---

## 📘 Conclusion  
This project demonstrates how simple metadata and text processing techniques can be used to create a functional content-based movie recommendation system. By applying vectorization and similarity analysis, the system successfully recommends movies that match the context and style of a given film.

---

## Author
**Fahiz Mohammed**
**LinkedIn:** www.linkedin.com/in/fahiz-mohammed-68130421b
