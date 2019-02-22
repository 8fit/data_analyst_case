# Data Analyst Case

## Requirements
* have a working installation of Docker
* use Python >=3.6

## Setup
* clone the repo
* install the requirements via `pip install -r requirements.txt`
* start the docker container by running `docker-compose up` (You prob. want to do this in a separate shell)
* `dbt seed --profiles-dir .`. This will create the necessary tables in the `dwh` schema which are relevant for solving this challenge.

## Links
* [DBT documentation](https://docs.getdbt.com/)
* [How to install Docker](https://docs.docker.com/install/)
