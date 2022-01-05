# Using Databases in Python

This repository is meant to provide a reference for how to connect to a [PostgreSQL](https://www.postgresql.org/) database, run SQL queries directly in a Jupyter notebook, then capture the result into a pandas dataframe for further analysis.

In order for the code in the Jupyter notebook to run properly, it requires several third-party Python packages. The following commands demonstrate how to create a virtual environment and install the relevant packages using [Anaconda](https://www.anaconda.com/):


```shell
conda create --name sql python
conda activate sql
conda install ipython-sql sqlalchemy psycopg2 notebook pandas -c conda-forge
```

The code utilizes a local PostgreSQL database populated with the Pagila example data (which is based on the MySQL Sakila example database). The `sql` files that create the schema and insert data can be found in the [Pagila GitHub repository](https://github.com/devrimgunduz/pagila). After cloning the repository, run the relevant file via `psql` or load the file directly into PGAdmin to recreate the database locally.
