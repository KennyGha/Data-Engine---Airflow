<h2> Airflow </h2>

<h3> Extract data from AWS S3 -> Airflow -> AWS Redshift  </h3>


Sparkify's Event Logs Data Pipeline
Introduction

This project consists of one Directed Acyclic Graph that implements the data pipeline responsible for reading all Sparkify's event logs, process and create some fact/dimensions tables described in our data schema down below.


![](dag.png)



For illustration purposes you can check out the graph that represents this pipeline's flow:

Directed Acyclic Graph of this Data Pipeline

Briefly talking about this ELT process:

    Stages the raw data;
    then transform the raw data to the songplays fact table;
    and transform the raw data into the dimensions table too;
    finally, check if the fact/dimensions table has at least one row.
