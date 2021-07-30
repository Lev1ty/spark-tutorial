# spark-tutorial

A tutorial on how to use PySpark on the Magarvey Lab computational server.

## Purpose

Apache Spark is a distributed computing platform written in Java and PySpark is the Python client library to access Apache Spark.
When your compute workload exceeds the memory capacity of computational server, consider browsing this tutorial to learn how to distribute your workload on the cluster.
In essence, Apache Spark decomposes your task into partitions and maps your algorithm onto each partition before collecting the partitions and performing aggregate computations.
Thus, ensure that your workload conforms to this compute paradigm.

## Install

1. Install Anaconda 3
2. Configure Anaconda 3 to prioritize `conda-forge` channel
  * `conda config --add channels conda-forge`
  * `conda config --set channel_priority strict`
3. Install and use `mamba` to parallelize `conda` operations
  * `conda install mamba --yes`
4. Install dependencies
  * `mamba install conda-pack pyspark --yes`
