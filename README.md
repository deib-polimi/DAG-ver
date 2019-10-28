## DAG-ver 

This repository provides additional information to the paper *"Using Formal Verification to Evaluate the Execution Time of Spark Applications"*.

### Dilworth's DAG Partitioning/labeling
Implementation of DAG labeling with Dilworth's theorem and Bogart-Magagnosc's algorithm
https://github.com/gioenn/dilworth-labeling 

The algorithm is integrated in the [D-VerT Tool](https://github.com/dice-project/DICE-Verification), which has been used to conduct the evaluation on the use cases.


### Evaluation
The xlsx files included in the  [docs](https://github.com/deib-polimi/DAG-ver/tree/master/docs) folder (downloadable through the links below) show the summary of the experiments carried out for the different use cases, highlighting the impact of the optimization in terms of both verification time and memory across the different verification tool configurations adopted.
Each file refers to a use case, and each sheet in the file refers to a tool configuration.

Each row in the tables shows the statistics regarding the verification of the feasibility problem against a specific deadline. 

The measures of interest are the **outcome** of verification&mdash;either **sat** (i.e. the set of formulae is *satisfied* for such deadline, therefore the deadline is feasible) or **unsat** (conversely, the set of formulae is *unsatisfiable*, and the deadline is not feasible)&mdash;, the verification time **v_time**, and the **memory** consumption. 
The suffixes **_opt** and **no_opt** identify if the measure refers to the optimized or to the non-optimized version of the model respectively.

![sample table](https://github.com/deib-polimi/DAG-ver/blob/master/docs/pagerank_sample_table.png?raw=true)

The impact on verification time is expressed in terms of ***speedup***. The value is the ratio between the smaller and the bigger of the two verification times with and without optimization, respectively. When the time needed to solve the optimized version is smaller, then there is a speedup, that is highlighted in the figures with a bar going from the center of the column to the right. On the other hand,  when the time to solve the non-optimized version is smaller, there is a slowdown (or negative speedup), represented in the figures with a negative sign and a bar going from the center to the left of the column. 

Analogously, the impact on memory is expressed in terms of ***memory saving***&mdash;that is, the percentage difference between the smaller and the bigger of the two memory consumption statistics with and without optimization, respectively. 
Positive values represent the percentage of memory that can be saved by using the optimization, while negative values express how much more memory (in percentage) is required by the optimized version with respect to the non-optimized one. 


To give anadditional visual overview about the comparison, table cells containting the values of *memory* and *v_time* are formatted to higlight which of the two version (optimized or non-optimized) performs better. We use a grayscale to indicate the entity of the relative improvement, with the following convention.

For *v_time*:
- light gray for speedup between 1.0x and 1.5x (respectively, slowdown between -1.0x and -1.5x)
- gray for speedup between 1.5x and 2.0x (respectively, slowdown between -1.5x and -2.0x)
- dark gray for speedup between 2.0x and 3.0x (respectively, slowdown between -2.0x and -3.0x)
- black for speedup above 3.0x (respectively, slowdown below -3.0x)

For *memory*:
- gray for percentage difference between 1% and 20% (respectively, between -1% and -20%)
- dark gray for percentage difference between 20% and 50% (respectively, between -20% and -50%)
- black for percentage difference above 50% (respectively, below -50%)
---

#### Download Links

[*SortByKey*](https://github.com/deib-polimi/DAG-ver/blob/master/docs/sort_by_key.xlsx?raw=true)

[*TPCH_22_6*](https://github.com/deib-polimi/DAG-ver/blob/master/docs/tpch_22_6n.xlsx?raw=true)

[*TPCH_22_7*](https://github.com/deib-polimi/DAG-ver/blob/master/docs/tpch_22_7n.xlsx?raw=true)

[*PageRank*](https://github.com/deib-polimi/DAG-ver/blob/master/docs/pagerank.xlsx?raw=true)

[*SVM*](https://github.com/deib-polimi/DAG-ver/blob/master/docs/svm.xlsx?raw=true)

[*K-means*](https://github.com/deib-polimi/DAG-ver/blob/master/docs/kmeans.xlsx?raw=true)

[*Louvain*](https://github.com/deib-polimi/DAG-ver/blob/master/docs/louvain.xlsx?raw=true)

---

Timing characteristics of the models are based on runs of the corresponding Spark applications profiled by means of [xSpark-Bench Tool](https://github.com/franco-maroni/xSpark-bench).

[D-VerT](https://github.com/dice-project/DICE-Verification) has been used to automate the model generation and verification process.

