# Failure-Dataset-OpenStack

This failure dataset contains information on the events collected in the **OpenStack** cloud computing platform during three different campaigns of **fault-injection** experiments performed with three different workloads (**DEPL**, **NET**, and **STO**).

The dataset contains three folders referring to the three different fault-injection campaigns (one per each workload).
In every folder, you can find:
* **SEQ.tsv**: a matrix with *N* rows and *d* columns containing the events collected during the fault-injection experiments. *N* is the number of fault-injection experiments, *d* represents the number of different event types (unique events).
* **LCS_with_VMM.tsv**: a matrix with *N* rows and *2d* columns containing the anomalies identified by the *LCS with VMM* approach during the fault-injection experiments. *N* is the number of fault-injection experiments, *d* represents the number of different event types (unique events). The first *d* columns (*1* to *d*) represent the number of spurious anomalies, the last d columns (*d+1* to *2d*) represents the number of missing anomalies.
* **Failure_Labels.txt**: a file containing the label class associated with every fault-injection experiment. The class label is expressed by a number. 

The number *N* of experiments and the number *d* of events depend on the workload used during the fault-injection experiments. Therefore, the matrix dimension in the *tsv* files change in every folder. 
We invite the reader to find further information on the data representation, the workloads, the anomaly types, and the failure classes by reading the paper [Enhancing the Analysis of Software Failuresin Cloud Computing Systems with Deep Learning](https://doi.org/10.1016/j.jss.2021.111043) accepted at the Journal of Systems and Software:

```
@article{cotroneo2021enhancing,
  title={Enhancing the analysis of software failures in cloud computing systems with deep learning},
  author={Cotroneo, Domenico and De Simone, Luigi and Liguori, Pietro and Natella, Roberto},
  journal={Journal of Systems and Software},
  volume={181},
  pages={111043},
  year={2021},
  publisher={Elsevier}
}
```

The slide presentation of the paper is available on [slideshare](https://www.slideshare.net/PietroLiguori4/enhancing-the-analysis-of-software-failures-in-cloud-computing-systems-with-deep-learning), while you can find the video presentation of the paper on [Youtube](https://www.youtube.com/watch?v=sQyol2aH-u0&list=PLhBMpvlFe-cHGnN9-9R5h2FWqjbBdyjA0&index=3&t=2s).

## Failure Classes
In our fault-injection experiments, we found different failure modes. We associated to each failure-mode a numeric value (**Failure Label**).

### DEPL
In the fault-injection campaing performed with the DEPL workload, the experiments experienced *6* different types of failures:

* **Failure Label 1**: *Instance Failure*
* **Failure Label 2**: *Volume Failure* 
* **Failure Label 3**: *SSH Failure* 
* **Failure Label 4**: *Cleanup Failure*
* **Failure Label 5**: *Network Failure* 
* **Failure Label 6**: *No Failure* 

### NET
In the fault-injection campaign performed with the NET workload, the experiments experienced *4* different types of failures:

* **Failure Label 1**: *Instance Failure*
* **Failure Label 2**: *Network Failure* 
* **Failure Label 3**: *SSH Failure* 
* **Failure Label 4**: *No Failure* 


### STO
In the fault-injection campaign performed with the DEPL workload, the experiments experienced *4* different types of failures:

* **Failure Label 1**: *Volume Failure* 
* **Failure Label 2**: *Instance Failure*
* **Failure Label 3**: *Cleanup Failure* 
* **Failure Label 4**: *No Failure* 
