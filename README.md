# Clustering-model
# Iris Dataset Clustering with K-Means
## Project Description
This project demonstrates unsupervised machine learning by applying K-Means clustering to the classic Iris dataset. The goal is to group iris flowers into clusters based on their sepal and petal measurements.

## Files
- `clustering.ipynb`: Jupyter Notebook containing the complete clustering analysis
- `iris.csv.xls`: Dataset file (150 iris samples with 4 features)

## Key Steps
1. **Data Loading & Exploration**:
   - Loaded the Iris dataset (150 samples × 6 features)
   - Checked for missing values (none found)
   - Examined data structure using `info()` and `describe()`

2. **Data Preparation**:
   - Selected features: `['SepalLengthCm', 'SepalWidthCm', 'PetalLengthCm', 'PetalWidthCm']`
   - Standardized data (if applicable)

3. **Clustering**:
   - Applied the Elbow Method to determine optimal clusters (k=3)
   - Implemented K-Means clustering with:
     ```python
     KMeans(n_clusters=3, init='k-means++', max_iter=300, n_init=10, random_state=0)
     ```
4. **Visualization**:
   - Created scatter plots showing:
     - Cluster assignments (3 colors)
     - Cluster centroids (yellow points)
   - Generated Elbow Method plot for cluster selection

## Requirements
- Python 3.x
- Libraries:
  ```bash
  pip install pandas numpy matplotlib scikit-learn jupyter
