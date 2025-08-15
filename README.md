🗂 Dataset

File: Mall_Customers.csv
Columns Used:

Annual Income (k$) → Customer's annual income in thousands of dollars.

Spending Score (1-100) → A score assigned by the mall based on customer spending behavior.

🛠 Tools & Libraries

Python 3

Pandas → Data handling

Matplotlib & Seaborn → Visualization

Scikit-learn → K-Means clustering, Silhouette Score, Scaling

📊 Steps Followed
1️⃣ Load & Explore the Dataset

Checked the first few rows to understand data structure and selected the two most relevant features for segmentation.

2️⃣ Data Preprocessing

Scaled the selected features (Annual Income & Spending Score) using StandardScaler to ensure all features have equal weight in clustering.

3️⃣ Finding Optimal K (Elbow Method)

Tried K values from 1 to 10.

Plotted Inertia vs. K to find the “elbow point” where adding more clusters doesn’t improve much.

4️⃣ Model Training (K-Means)

Chose K = 5 (based on Elbow Method).

Fitted K-Means and assigned each customer to a cluster.

5️⃣ Evaluation

Calculated Silhouette Score to check how well clusters are separated.

6️⃣ Visualization

Scatter plot of clusters with different colors.

Plotted cluster centroids for better interpretation.

📈 Results

Optimal K: 5

Silhouette Score: ~0.55 (good separation)

Clear groups of customers emerged:

Low Income – Low Spending

Low Income – High Spending

Medium Income – Medium Spending

High Income – Low Spending

High Income – High Spending
