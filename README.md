# Netflix-Content-Clustering

**A data mining project analyzing Netflix movies and TV shows using clustering techniques.**

---

## Project Overview
This project applies **unsupervised learning** to Netflix data to discover hidden patterns in movies and TV shows. Using **K-Means** and **Agglomerative Clustering**, we analyze features such as genres, release year, ratings, and duration to uncover meaningful content groups.

---

## Dataset
- **Source:** [Kaggle – Netflix Movies and TV Shows](https://www.kaggle.com/code/bansodesandeep/netflix-movies-and-tv-shows-clustering/input)
- **Features include:**  
  - `type` — Movie or TV Show  
  - `title` — Title of the content  
  - `director` — Director(s)  
  - `cast` — Main cast  
  - `country` — Country of production  
  - `date_added` — Date added to Netflix  
  - `release_year` — Year of release  
  - `rating` — Content rating  
  - `duration` — Duration in minutes or seasons  
  - `listed_in` — Genres/categories

---

## Steps / Workflow
1. **Load and clean the dataset** — handle missing values, duplicates, and strip whitespace.
2. **Preprocessing** — encode categorical features (`type`, `rating`), convert `duration` to numeric, one-hot encode genres.
3. **Feature scaling** — use `StandardScaler` to normalize features.
4. **Clustering**  
   - **K-Means Clustering** — assign each title to a cluster.  
   - **Agglomerative Clustering** — compare with K-Means clusters.  
5. **Evaluation** — compute **silhouette scores** and **Adjusted Rand Index**.  
6. **Cluster profiling & visualization** — examine top genres, average release year, type distribution, and durations.  
7. **Optional** — PCA visualization to see clusters in 2D space.

---

## Insights
- Clusters reveal content patterns, e.g., groups dominated by TV shows vs. movies, specific genres, or release periods.  
- Can be used to improve recommendation systems, inform content strategy, and explore hidden content groupings.

---

## How to Run
1. Clone the repository:  
   ```bash
   git clone https://github.com/yourusername/Netflix-Content-Clustering.git
