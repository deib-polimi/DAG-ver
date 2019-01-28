### Evaluation of the optimized models

These xlsx files show the summary of the experiments carried out for the different use cases, highlighting the impact of the optimization in terms of both verification time and memory across the different verification tool configurations adopted.
Each file refers to a use case, and each sheet in the file refers to a tool configuration.

Each row in the tables shows the statistics regarding the verification of the feasibility problem against a specific deadline. 

The measures of interest are the **outcome** of verification&mdash;either **sat** (i.e. the set of formulae is *satisfied* for such deadline, therefore the deadline is feasible) or **unsat** (conversely, the set of formulae is *unsatisfiable*, and the deadline is not feasible)&mdash;, the verification time **v_time**, and the **memory** consumption. 
The suffixes **_opt** and **no_opt** identify if the measure refer to the optimized and non-optimized version of the model respectively.

For each deadline 
![sample table](https://github.com/deib-polimi/DAG-ver/blob/master/docs/pagerank_sample_table.png?raw=true)

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
