# Machine Learning (NBA Players CLustering)

Created and tuned a machine learn model to group players in clusters, ideal number of clusters was found using elbow method and by creating a dendrogram.
The dataset was gotten from Kaggle and consisted of 11,145 rows and 21 columns. It contained stats for each player from the 1996 season until the 2019 season.

Exploratory analysis was conducted to familiarize myself with the dataset.

---

## Making the Clusters

To begin, I needed to determine the optimal number of clusters I used the elbow method.

![](/elbow_method.jpg)

---

To check myself I created a dendrogram.

![](/dendrogram.jpg)

---

I used K-means to cluster the data into 3 groups. I then compared each cluster against one another.

![](/figure1.jpg)

---

I then wanted to find out how the clusters were formed. I used .describe() on each cluster to look at the averages, and found that clusters might be created based on games played and position.
To check I looked at some of the most notable players from each group.

---

### Cluster 0: Contained players that didn't play most of the season (injuries)

![](/cluster0_players.jpg)

---

### Cluster 1: Contained many points guards, shooting guards, and some small forwards.

![](/cluster1_players.jpg)

---

### Cluster 2: Contained small forwards, power forwards, and centers.

![](/cluster2_players.jpg)

---
The scatterplot shows games played on the x axis and height on the y axis. Each cluster is color coated.

![](/figure2.jpg)

