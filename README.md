# 🎬🤖 Movie Recommendation System using Content-Based Filtering

This project recommends movies based on their **genres, cast, director, keywords**, and **tagline** using **content-based filtering**. It applies **TF-IDF vectorization** and **cosine similarity** to find and suggest similar movies based on the user's input. This helps users discover new films that match their preferences.

---

## 📄 Dataset

- **Source:** [Movie Dataset (Google Drive)](https://drive.google.com/file/d/1cCkwiVv4mgfl20ntgY3n4yApcWqqZQe6/view)
- **Description:** The dataset contains movie metadata, including:
  - `title` – Movie name
  - `genres` – Genre of the movie
  - `keywords`, `tagline`, `cast`, `director` – Descriptive text features for each movie

---

## ⚙️ Technologies Used

- Python  
- NumPy  
- Pandas  
- Scikit-learn (TfidfVectorizer, Cosine Similarity)
- Difflib (String Matching)

---

## 📊 Project Workflow

### 1️⃣ Data Loading & Preprocessing
- Load dataset using Pandas.
- Select features: `genres`, `keywords`, `tagline`, `cast`, and `director`.
- Fill missing values with empty strings.

### 2️⃣ Feature Combination
- Combine selected features into a single string per movie.

### 3️⃣ Vectorization
- Use **TfidfVectorizer** to convert text data into feature vectors.

### 4️⃣ Similarity Calculation
- Compute **cosine similarity** between all movie vectors.

### 5️⃣ Movie Matching
- Accept movie name input from the user.
- Use **difflib** to find the closest match in the dataset.

### 6️⃣ Recommendation Output
- Retrieve and display top 30 movies with the highest similarity scores.

---

## ✅ Results

- The system efficiently recommends content-similar movies based on the user's input.
- Delivers personalized recommendations within seconds.

---

## 🔍 Example Recommendation

**User Input:**  
🎥 *Avengers: Endgame*

**Top Suggestions:**  
1. Avengers: Infinity War  
2. Captain America: Civil War  
3. Iron Man 3  
4. Thor: Ragnarok  
5. Guardians of the Galaxy  
… and more!

---

## 💡 Key Learnings

- How to process and clean movie metadata.
- Feature engineering by combining multiple textual features.
- TF-IDF vectorization and cosine similarity concepts.
- Building a recommendation system without user rating data.

---

## 📥 How to Run

1️⃣ **Clone this repository:**

```bash
git clone https://github.com/Princegupta-78/Movie-Recommendation-System.git
```

2️⃣ **Install dependencies:**
```bash
pip install numpy pandas scikit-learn
```

3️⃣ **Run the notebook:**
```bash
jupyter notebook Movie_Recommendation_System.ipynb
```