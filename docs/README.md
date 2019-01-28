### Evaluation of the optimized models

The files show the summary of the experiments carried out for the different use cases, highlighting the impact of the optimization in terms of both verification time and memory across the different verification tool configurations adopted.

Each row in the tables shows the statistics regarding the verification of the feasibility problem against a specific deadline. The ***deviation*** column  indicates the percentage difference between the ***deadline*** of the row and the *minimum feasible deadline found (**mfd<sub>f</sub>**)* for that specific use case setting, and expresses how much the deadline is higher or lower (negative percentage values) than the *mfd<sub>f</sub>*.

The impact on verification time is expressed in terms of ***speedup***. The value is the ratio between the smaller and the bigger of the two verification times with and without optimization, respectively. When the time needed to solve the optimized version is smaller, then there is a speedup, that is highlighted in the figures with a bar going from the center of the column to the right. On the other hand,  when the time to solve the non-optimized version is smaller, there is a slowdown (or negative speedup), represented in the figures with a negative sign and a bar going from the center to the left of the column. 

Analogously, the impact on memory is expressed in terms of ***memory saving***&mdash;that is, the percentage difference between the smaller and the bigger of the two memory consumption statistics with and without optimization, respectively. 
Positive values represent the percentage of memory that can be saved by using the optimization, while negative values express how much more memory (in percentage) is required by the optimized version with respect to the non-optimized one. 

#### Download Links

[*SortByKey*](https://github.com/deib-polimi/DAG-ver/blob/master/docs/sort_by_key.xlsx?raw=true)

[*TPCH_22_6*](https://github.com/deib-polimi/DAG-ver/blob/master/docs/tpch_22_6n.xlsx?raw=true)

[*TPCH_22_7*](https://github.com/deib-polimi/DAG-ver/blob/master/docs/tpch_22_7n.xlsx?raw=true)

[*PageRank*](https://github.com/deib-polimi/DAG-ver/blob/master/docs/pagerank.xlsx?raw=true)

[*SVM*](https://github.com/deib-polimi/DAG-ver/blob/master/docs/svm.xlsx?raw=true)

[*K-means*](https://github.com/deib-polimi/DAG-ver/blob/master/docs/kmeans.xlsx?raw=true)
