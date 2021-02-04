# Failure-Dataset-OpenStack

This failure dataset contains the events collected in the **OpenStack** cloud computing platform during three different campaigns of **fault-injection** experiments performed with three different workloads (DEPL, NET and STO).

The dataset contains three folders referring to the different fault-injection campaigns.
In every folder, you can find:
* **SEQ.tsv**: a matrix with N rows and d columns containing the events collected during the fault-injection experiments. N is the number of fault-injection experiments, d represents the number of different event types (unique events).
* **LCS_with_VMM.tsv**: a matrix with N rows and 2d columns containing the anomalies identified by the LCS with VMM approach during the fault-injection experiments. N is the number of fault-injection experiments, d represents the number of different event types (unique events). The first d columns (1 to d) represent the number of spurious anomalies, the last d columns (d+1 to 2d) represent the number of missing anomalies.
* **Failure_Labels.txt**: a file containing the label class associated to every fault-injection experiment. The class label is experessed by a number. 

We invite the reader to find further information on the data representation, on the workloads and on the failure classes by reading the paper:  




Please, **cite the paper** if you use the dataset for your research:

```
```
