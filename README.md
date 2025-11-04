# KMeans Clustering From Scratch

Welcome to the **KMeans Clustering By Scratch** repository!  
This project offers a complete implementation of the KMeans clustering algorithm using only core Python, without relying on machine learning libraries such as scikit-learn. It's a great resource for understanding the inner workings of this foundational unsupervised learning algorithm.

## Features

- **No External ML Libraries:** All clustering logic is written from scratch.
- **Educational:** Designed to illustrate each step of the KMeans process for learning and experimentation.
- **Customizable:** Code can be easily extended for additional features or enhancements.

## Getting Started

1. **Clone the repository:**
   ```sh
   git clone https://github.com/GalaxyMatrix/Kmeans_clustering-by-scratch.git
   cd Kmeans_clustering-by-scratch
   ```

2. **Requirements:**
   - Python 3.x
   - [Optional] matplotlib, numpy for data handling and visualization (if the code includes visualization)

   Install (if needed):
   ```sh
   pip install numpy matplotlib
   ```

3. **Running the Code:**
   - Open and run the main Python script (e.g., `kmeans.py`):
     ```sh
     python kmeans.py
     ```

## Example Usage

```python
from kmeans import KMeans

# Example data
X = [
    [1.0, 2.0],
    [1.5, 1.8],
    [5.0, 8.0],
    [8.0, 8.0],
]

# Initialize KMeans and fit to the data
k = 2
model = KMeans(n_clusters=k)
model.fit(X)

print("Centroids:", model.centroids)
print("Labels:", model.labels_)
```

_For more examples, see the example scripts or notebook in this repository._

## Project Structure

```
kmeans_clustering-by-scratch/
├── kmeans.py           # Core KMeans implementation
├── dataset.csv         # Sample dataset (if available)
├── README.md           # This documentation
├── ...
```

## How KMeans Works

1. **Initialization:** Randomly select `k` centroids.
2. **Assignment:** Assign each data point to the nearest centroid.
3. **Update:** Compute new centroids as the mean of all points assigned to each.
4. **Repeat:** Iterate the assignment and update steps until convergence.

## License

This project is licensed under the MIT License.

---

**Author:** [GalaxyMatrix](https://github.com/GalaxyMatrix)

Contributions, issues, and feature requests are welcome!
