# A Novel Approach to Outlier-Aware K-means Clustering
Clustering algorithms like k-means often struggle to classify data containing outliers, as these extreme values can distort centroid calculations. To address this limitation, we developed an outlier-aware k-means algorithm that integrates both k-means and k-medians using a weighted mean. The weight is calculated based on the ratio of high outliers to the total size of the dataset, amplified by a cube root function to enhance k-medians’ influence when extreme values are present. The model was evaluated on a synthetic dataset of 450 instances and two quantitative continuous features, generated using scikit-learn’s make_blobs function. Compared to traditional k-means, the outlier-aware algorithm achieved higher accuracy (0.9044 vs. 0.8978), precision (0.9115 vs. 0.9065), recall (0.9140 vs. 0.9080), and F1-score (0.9044 vs. 0.8978). The results demonstrate that the adaptive weighting strategy effectively balanced outlier resistance and accurate centroid placement, leading to more consistent cluster boundaries. In the future, we will explore the scalability of this algorithm on higher-dimensional datasets and investigate other weighting strategies.

**How to Run:**
1. Open Q2_Project.ipynb in Google Colab
2. Upload the file q2_project_data.csv in the Colab environment
3. Hover over "Runtime" in the top bar and click "Run all"
