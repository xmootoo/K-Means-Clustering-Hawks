# K-Means Clustering (Hawks)

This is a script designed to classify hawk species with unsupervised learning by k-means clustering in R.

The ‘hawks’ dataset was retrieved from: https://vincentarelbundock.github.io/Rdatasets/datasets.html

More info: https://vincentarelbundock.github.io/Rdatasets/doc/Stat2Data/Hawks.html


In total, the dataframe contained 908 observations and 19 variables with 3 different hawk species: Red-tailed, Sharp-Shinned, and Cooper's. 

Variables selected for k-means clustering were chosen for relevance to potential hawk-specific phenotypes and for variables with the least amount of missing values in the dataset.

Data was then clustered on these 5 dimensions: Weight (g), Wing (mm), Culmen (mm), Hallux (mm) and Tail (mm). 
Seed was set to 1000 and k = 3 (one cluster for each species), and after the k-means algorithm was finished assigning clusters, a cluster count table was recorded with respect to each species.

I was exploring visualizations 3D scatterplots with plotly as well, so I created a 3D visualization using only 3 of the 5 dimensions used in the k-means clustering: 
wing length, culmen length and weight; each datapoint was coloured by the respective cluster.
