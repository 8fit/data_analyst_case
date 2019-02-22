# Data Analyst Case
Thanks a lot for taking the time to tackle the challenge for the Data Analyst role here at 8fit.

## Requirements

* have a working installation of Docker
* use Python >=3.6

## Setup

* clone the repo
* install the requirements via `pip install -r requirements.txt`
* start the docker container by running `docker-compose up` (You prob. want to do this in a separate shell)
* `dbt seed --profiles-dir .`. This will create the necessary tables in the `dwh` schema which are relevant for solving this challenge.

## Data

You will find 2 tables in your `dwh` schema:
* `subscriptions`
* `spendings`

Let's assume that you're looking at data from Q4/2016 and 01/2017

## Analysis Scenario
Imagine our Head of Performance Marketing sends you an email:

> I need to understand where to invest more money. I'm curious if you can help me make a decision based on your findings. Do you think it's ios or android?
>
> Aside from that I'm also curious if there's specific marketing channels we should be aiming for to get better results? I'm currently thinking that the channel with ID 4 looks promising. What are your thoughts?
> Looking further into the data at hand it looks like UK (United Kingdom) would be a good investment. Do you agree?

> It would be great if you can present your findings and suggestions next week at the weekly marketing staff meeting.

> Thanks,
> Ben

### Task
Please compile a presentation about these questions. Feel free to use the tools you prefer to explore, analyse and visualise the data.

For easiest reading we'd appreciate if you add a PDF version of the presentation in the `analysis` folder inside the repository. Please also place any meaningful intermediate steps, explorations and documentation into the same folder so we can review your work.

## SQL experience


## Links

* [DBT documentation](https://docs.getdbt.com/)
* [How to install Docker](https://docs.docker.com/install/)
