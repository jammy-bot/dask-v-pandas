# Computation Acceleration with Dask vs Pandas 
Exploring speed advantages realized by using the Dask library over Pandas for dataframe operations in Python.

<img src="https://github.com/jammy-bot/dask-v-pandas/blob/master/images/panda-306265_1280.png" width="365" height="448" title="Github Logo">

## Introduction
Dask is a framework that enables Pandas, Scikit-Learn, and Numpy to scale beyond a single machine to work over multiple clusters, while using a familiar API. At the same time, Dask facilitatates rapid, parallel computation on single - machine CPUs.  

## Objectives
I wanted to get an idea for how much faster I might be able to perform dataframe operations on a multi - core, Intel i7 CPU outfitted laptop pc.

## The Dataset
For the project, I produced a million - rows of randomly generated stock prices and converted the data into a Pandas dataframe. I then exported the data to a CSV and loaded it into a Dask Dataframe.

## The Task(s)
I performed the same operations on each dataframe and compared their computation durations. I tested calculating dataframe means across all rows, filtering all rows on a threshold, and adding the complete dataframe to itself five times. The operations were computed and timed for one, 10 thousand (10K), and 100K iteration(s).

## Results
    - Calculating the mean of randomly generated stock prices across 1M rows proved to be about 17.6\% slower for 100K iterations, with Dask.
    - Filtering across the same dataset is about 96\% faster for 100K iterations, with Dask.
    - Adding together 5 copies of the dataset for 10K iterations is about 95\% faster, with Dask--just over 3 minutes, as opposed to more than an hour with pandas.
        - Adding dataframes for 100K iterations with Dask completed in *** minutes.

## Future Work
> GPU
* PC
* Containerized
* Cloud CPU / GPU

====================================================================
