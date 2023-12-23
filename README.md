# Bossabyte Airflow

This repo stores the airflow configuration and DAGs for the Bossabyte project.


## How to start the delevopment

- Download astro cli `curl -sSL install.astronomer.io | sudo bash -s`
- On the Dags folder, each project folder is a git submodule pointing to another repo.
- Write your Python modules and DAG code on your repo, it will be automatically reflected on the airflow repo
- To test your DAGs code, run `astro run <dag_name>` (your DAG name is the name of the DAG file without the `.py`) , i.e `astro run example_dag_basic`