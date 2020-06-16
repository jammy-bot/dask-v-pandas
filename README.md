# dask-v-pandas
Exploring speed advantages realized by using the Dask library over Pandas for dataframe operations in Python.

> i7 PC
* CPU
    - Calculating the mean of randomly generated stock prices across 100,000 rows is about 17.6\% slower with Dask.
    - Filtering across the same dataset is about 94.7\% faster with Dask.
    - Adding together 5 copies of the dataset is about ***\% faster with Dask.
* ...On GPU

> Containerized
