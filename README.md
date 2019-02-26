# Data Analyst Case
Thanks a lot for taking the time to tackle the challenge for the Data Analyst role here at 8fit.

While you work your way through this case you will most likely have questions, find problems or even things not working out. If you encounter anything please do not hesitate to reach out to us and we'll help you out. We all make mistakes and can learn from each other :sun:

## Requirements

* have a working installation of Docker
* use Python >=3.6

## Setup

* fork the repo to your own account on Github, Bitbucket or Gitlab
* clone the repo
* install the requirements via `pip install -r requirements.txt`
* start the docker container by running `docker-compose up` (You prob. want to do this in a separate shell)
* `dbt seed --profiles-dir .`. This will create the necessary tables in the `dwh` schema which are relevant for solving this challenge. This can take some minutes to finish!
* You should see the following output in your terminal once the seeding of the data was successful:
    ```
    $ dbt seed --profiles-dir .
    Found 0 models, 0 tests, 0 archives, 0 analyses, 95 macros, 2 operations, 2 seed files

    13:17:32 | Concurrency: 1 threads (target='dev')
    13:17:32 |
    13:17:32 | 1 of 2 START seed file dwh.spendings................................. [RUN]
    13:20:04 | 1 of 2 OK loaded seed file dwh.spendings............................. [INSERT 623979 in 85.21s]
    13:20:04 | 2 of 2 START seed file dwh.subscriptions............................. [RUN]
    13:20:11 | 2 of 2 OK loaded seed file dwh.subscriptions......................... [INSERT 29823 in 4.00s]
    13:20:11 |
    13:20:11 | Finished running 2 seeds in 158.80s.

    Completed successfully

    Done. PASS=2 ERROR=0 SKIP=0 TOTAL=2
    ```
* If you want to use your tooling of choice you can connect to the PG instance running in the docker container using the following credentials:
    ```
    user: data_analyst_case
    password: data_analyst_case
    database: data_analyst_case
    port: 5432
    host: 127.0.0.1
    ```

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
>
> It would be great if you can present your findings and suggestions next week at the weekly marketing staff meeting.
>
> Thanks,
> Ben

### Task
Please compile a presentation about these questions. Feel free to use the tools you prefer to explore, analyse and visualise the data.

For easiest reading we'd appreciate if you add a PDF version of the presentation in the `analysis` folder inside the repository. Please also place any meaningful intermediate steps, explorations and documentation into the same folder so we can review your work.

## SQL experience

Please write down the queries to answer the following questions:

### 1. How much did we spent per channel in December?
### 2. What is the average cost of acquisition for a subscription per country?
### 3. What is our average revenue and spending per day of the week (Monday, Tuesday...)?

You can either use DBT models to answer these questions or write plain SQL and add them to the `analysis` folder within the repo.

## Deliver your solution
Once you feel comfortable with your solution and you've committed the necessary bits to your own fork, get back to us again via email. In this email please add a link to your own fork. Keep in mind that we want to understand and validate your solution so please add any kind of documentation you want into the repo.

Again thanks for your time to work on this case.

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

Please write down the queries to answer the following questions:

> How much did we spent per channel in December ?

> What is the average cost of acquisition of a subscription per country ?

> What is our average revenue and spends per day of the week (Monday, Tuesday...) ?

## Links

* [DBT documentation](https://docs.getdbt.com/)
* [How to install Docker](https://docs.docker.com/install/)
