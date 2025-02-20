# 📚 Book Recommendation Engine

## 📌 Overview

This project implements a **Book Recommendation System** using **K-Nearest Neighbors (KNN)** and collaborative filtering. The model suggests books similar to a given book based on user ratings. The dataset used is the **Book-Crossing Dataset**, which includes book titles, authors, and user ratings.

## 📊 Dataset

- **Source**: [Book-Crossing Dataset](https://cdn.freecodecamp.org/project-data/books/book-crossings.zip)
- **Files Used**:
  - `BX-Books.csv`: Contains book details (ISBN, title, author)
  - `BX-Book-Ratings.csv`: Contains user ratings for books
- **Data Processing**:
  - Filter users with at least **200 ratings**
  - Filter books with at least **100 ratings**
  - Convert dataset into a **pivot table**
  - Transform the pivot table into a **sparse matrix**

## ⚙️ Technologies & Skills Used

- **Machine Learning**: K-Nearest Neighbors (KNN) Algorithm
- **Data Preprocessing**: Filtering, data transformation, and sparse matrices
- **Python Programming**: NumPy, Pandas, Matplotlib
- **Scikit-Learn**: Implementing KNN model
- **Collaborative Filtering**: User-based recommendation system

## 🚀 Project Workflow

1. **Data Loading & Preprocessing**
   - Read book details and ratings datasets
   - Filter users and books based on the number of ratings
   - Create a **pivot table** and fill missing values with zero
2. **Model Training**
   - Convert the pivot table into a **sparse matrix**
   - Train a **K-Nearest Neighbors (KNN)** model using cosine similarity
3. **Generating Recommendations**
   - Find similar books for a given book title
   - Return the top 5 book recommendations along with similarity scores

## 📈 Results

- The system successfully recommends **5 books** similar to a given book title.
- Uses **cosine similarity** to measure book similarity.
- Provides a scalable approach to book recommendations.

## 🔧 How to Run

1. Install dependencies:
   ```bash
   pip install numpy pandas matplotlib scikit-learn
   ```
2. Run the Python script:
   ```python
   python book_recommendation.py
   ```
3. Call the function:
   ```python
   get_recommends("Where the Heart Is (Oprah's Book Club (Paperback))")
   ```

## 📌 Future Improvements

- Implementing **Content-Based Filtering** for recommendations.
- Improving performance by using **approximate nearest neighbors (ANN)**.
- Enhancing recommendation quality with **hybrid filtering techniques**.

## 🏆 Acknowledgments

- FreeCodeCamp for providing the dataset
- Scikit-Learn for KNN implementation

---

### 🌟 **Contributions**

Feel free to fork the repository and contribute improvements. If you have suggestions, open an issue or submit a pull request!

