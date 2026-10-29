# The_Karate_Club_Graph

In this assignment, the objective is to discover groups of people who are more strongly connected to each other than we would expect by chance i.e "Community Detection". The algorithm used to do that uses a mathematical quantity called 'modularity' and the graph used is 'Zachary's Karate Club graph'. It:

1. At each iterations builds the modularity matrix for all communities (at i=0 the original graph itself) and checks its basic properties.
2. Splits a community in two(Spectral bipartition algorithm) using the sign of the leading eigenvector of its restricted matrix
3. Applying the algorithm after each community split to each group until no community has a positive leading eigenvalue (i.e. a usable sign split)
4. Illustrate the full graph after every split, giving each community a different color
5. Calculate centrality like degree centrality, betweenness centrality, closeness centrality and the clustering coefficient for every node after each split, and plots how each metric evolves
6. Compares the detected communities after the algorithm finishes;
