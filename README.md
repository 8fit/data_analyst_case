# Data Analyst Case

## Requirements

* have a working installation of Docker
* use Python >=3.6

## Setup

* clone the repo
* install the requirements via `pip install -r requirements.txt`
* start the docker container by running `docker-compose up` (You prob. want to do this in a separate shell)
* `dbt seed --profiles-dir .`. This will create the necessary tables in the `dwh` schema which are relevant for solving this challenge.

## Data

You will find 2 tables in your `dwh`schema:

* `subscriptions` table
* `spendings` table

## Analytical Questions

**1) Our Head of Performance Marketing is asking you: In which platform should I invest more money (ios or android)?**

**2) Our Head of Performance Marketing says: ok! but should I spend more in an specific marketing channel for this platform, maybe Facebook?**

**3) Our Head of Performance Marketing says: ah! I have the intuition that United Kingdom will be a great investment, do you agree?**

You are free to choose your favorite toolset (SQL queries, Tableau, Metabase, ipython, excel...) in order to explore, analyse and visualise the data.

The final document could be a powerpoint, a word document or a ipython notebook.

## SQL Quetions


## Links

* [DBT documentation](https://docs.getdbt.com/)
* [How to install Docker](https://docs.docker.com/install/)
