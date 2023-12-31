# Bossabyte Airflow

This repo stores the airflow configuration and DAGs for the Bossabyte project.


## How to start the delevopment

- Download astro cli `curl -sSL install.astronomer.io | sudo bash -s`
- On the Dags folder, each project folder is a git submodule pointing to another repo.
- To add a submodule on the `dags/` folder, run ` git submodule add https://github.com/bossabyte/ALERJ.git`
- Write your Python modules and DAG code on your repo, it will be automatically reflected on the airflow repo
- To test your DAGs code, run `astro run <dag_name>` (your DAG name is the name of the DAG file without the `.py`) , i.e `astro run example_dag_basic`

- To pull the latest changes on the submodules to the Airflow repo, run `git submodule update --recursive --remote --force`

Note: Don't push changes to the submodules via the Airflow repo, use an individual clone of each module to push changes.