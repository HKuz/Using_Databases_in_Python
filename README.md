# Using Databases in Python

In order for the code in the Jupyter notebook to run properly, it requires several third-party Python packages. The following commands demonstrate how to create a virtual environment and install the relevant packages using [Anaconda](https://www.anaconda.com/).


```shell
conda create --name sql python
conda activate sql
conda install ipython-sql sqlalchemy psycopg2 notebook pandas -c conda-forge
```

The code utilizes a local [PostgreSQL](https://www.postgresql.org/) database with the Pagila example data (based on the popular MySQL Sakila example database). After cloning the [repository for the Pagila example database](https://github.com/devrimgunduz/pagila) off GitHub, run the `.sql` script via `psql` or load the file directly into PGAdmin to recreate the database locally.
