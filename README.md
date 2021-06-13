# grading-algo-clustering
Grading of marks data done using k-means clustering

**Details**

The algorithm, based on the research and survey we conducted, will take students’ marks as input and assign them the grades. The algorithm is a hybrid technique which is a combination of absolute grading, relative grading and K-means clustering. For determining optimal number of clusters, we are using Silhouette method. 

**Evaluation Criteria of Algorithm**

•	Less than a minimum marks, say 33, will result in F.

•	No A+ below a maximum, say 90.

•	There shall be a gap between any two grades.

•	Grade at average shall be either B- or C+.

•	F and A+ shall lie outside the first standard deviation.

•	The algorithm shall use most of the grades.

•	The number of students in each bucket/cluster/grade shall not vary significantly.

**Algorithm** 

1.	First threshold data with maximum and minimum marks for A+ and F respectively.
2.	Find the optimal number of clusters using some method (say Silhouette Score).
3.	Then provide the number of k to clustering obtained from step 2.
4.	After applying clustering, find the cluster which contains the average value of the data (for giving average grade).
5.	Then, clusters before this cluster will get grades from B to A and clusters after the average cluster will get grades from C+ to D.

**Silhouette Score on a sample marks data**

![image](https://user-images.githubusercontent.com/60185211/121815075-dfac5400-cc8d-11eb-934e-200f7fb7dfa3.png)

**Clustering based on optimal Silhouette Score**

![image](https://user-images.githubusercontent.com/60185211/121815091-ee930680-cc8d-11eb-9bf1-913fe139782c.png)
