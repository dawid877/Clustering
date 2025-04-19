# Songs Clustering Project

The goal of this project is to perform clustering analysis on the weekly Top 200 songs from Spotify, using data obtained via the Spotify API.

Several clustering algorithms were applied:
- K-Means
- Hierarchical Clustering
- Partitioning Around Medoids (PAM)
- DBSCAN (Density-Based Spatial Clustering of Applications with Noise)

To improve clustering performance, dimensionality reduction was performed using **Principal Component Analysis (PCA)**.  
Cluster evaluation was conducted using **Silhouette Score** and **Hopkins Statistic**.

## Tech stack
- **Language:** R  
- **Key Packages:** `spotifyr` (Spotify API), `factoextra`, `cluster`, `dbscan`, `clustertend`, `plotly`

## Project Structure
**Main_code/**  
- `Clustering_project.ipynb` – The core R code in Jupyter Notebook format.  
- `Clustering_project_html.html` – Exported HTML version of the notebook.  
  **Note:** The 3D visualizations will *not* render in this format.

**Data/**  
- `regional-global-weekly-2024-12-19.csv` – Raw dataset of Spotify's Top 200 songs for the week of Dec 12–19, 2024.  
- `top200.csv` – Cleaned and preprocessed version used in the analysis.  
  **Note:** This file must be in the same directory when running the `.ipynb` notebook.  
- `final_scaled_data.csv` – Scaled numerical features used for clustering.
