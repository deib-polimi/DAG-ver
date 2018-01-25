## DAG-ver 

This repository provides additional information to the paper *"Optimizing the Timed Analysis of ordered DAG-based computations"*.

### Dilworth's DAG Partitioning/labeling
Implementation of DAG labeling with Dilworth's theorem and Bogart-Magagnosc's algorithm
https://github.com/gioenn/dilworth-labeling 

The algorithm is integrated in the [D-VerT Tool](https://github.com/dice-project/DICE-Verification), which has been used to conduct the evaluation on the Apache Spark use case.


### Evaluation
Evaluation has been performed on four different use cases for two different formalisms: CLTLoc and TA.
* CLTLoc experiments have been carried out by using the Zot formal verification tool. More details on the experiments can be found [here](https://github.com/deib-polimi/DAG-ver/wiki/FM2018-Evaluation-Zot)
* TA experiments have been carried out by means of the UPPAAL formal verification tool. More details on the experiments can be found [here](https://github.com/deib-polimi/DAG-ver/wiki/FM2018-Evaluation-Uppaal)

Timing characteristics of the models are based on runs of the corresponding Spark applications profiled by means of [xSpark-Bench Tool](https://github.com/franco-maroni/xSpark-bench).

[D-VerT](https://github.com/dice-project/DICE-Verification) has been used to automate the model generation and verification process.

