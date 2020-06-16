# dask-v-pandas
Exploring speed advantages realized by using the Dask library over Pandas for dataframe operations in Python.

> i7 PC
* CPU
    - Calculating the mean of randomly generated stock prices across 1M rows is about 17.6\% slower for 100K iterations, with Dask.
    - Filtering across the same dataset is about 95\% faster for 100K iterations, with Dask.
    - Adding together 5 copies of the dataset for 10K iterations is about 95\% faster, with Dask.
* ...On GPU

> Containerized
