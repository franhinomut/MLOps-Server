# **MLOps Server**

💡 Overview of a **MLOps Server** created using **Airflow, mlflow, Jupyter and Postgres.**

In the project we will use jupyter to generate pipelines that airflow is able to process. What we create with jupytes will be visible from Airflow. Mlfow will be in charge of running machine learning experiments. In Postgres we will store all the data generated.

## 🤖 **Instructions**

1 - The first thing to do is to clone the project from the degithub repository: 

    `git clone https://github/franhinomut/mlops-server.git`

2 - **docker-compose.yaml** This is a **YAML file** that defines the services, networks and volumes for a **Docker application**. The file specifies the dependencies between the servicies an how to run the containers:

In our case, we are going to install several images necessary to install an MLOps server:

    - Jupyter, an application that will allow us to run notebooks locally, which uses port 8888, 
    - Airflow on port 8080, which we will use to manage and handle code pipelines,
    - mlflow, which uses port 5000
    - postgres databases, which use ports 5432, 5433

Let's run the following code to assemble all the modules of the project: 

    `docker compose up`