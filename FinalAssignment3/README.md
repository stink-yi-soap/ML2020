Option 2: Clustering Image Metadata

I clustered the images based on "art_movement", "primary_medium", "representation", "te"(texture of the artwork), "sh"(the shape of marks), "li"(qualities of lines). 
Then I replaced the missing values in the data set with 0, and transformed strings in "art_movement" and "primary_medium" by assigning them numerical keys. 

The inertia plot shows an elbow around n=10, but when I reviewed the images in each cluster, the clusters seemed too big that it was hard to tell the commonality within each cluster. So I tested different n values between 10 and 40, and eventually set n=32 for my model. With 32 clusters, some clusters are exhibiting satisfactory curation, and the strength and weakness of this model is becoming apparent. 

For instance, cluster 0, 1 and 7 are all brought together by the formal qualities of the art work, particularly in the lines and mark-making. Since I chose "te", "sh" and "li" as data points, this model seems more adept at clustering modern+contemporary art, especially non-representational art. 

In contrast, cluster 9 exemplifies how this model fails to curate classical art in sensible ways. No matter what n value I set, the classical paintings are always arbitrarily thrown into different clusters. 

This model often makes a decent curation of surrealist art and ready-made sculptures, as demonstrated in cluster 11, 22 and 23. It doesn't seem to do nearly as well with other art movements. 

