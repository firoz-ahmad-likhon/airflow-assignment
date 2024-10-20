## Introduction
It is an assignment to collect Actual or estimated wind and solar power generation data from  [here](https://bmrs.elexon.co.uk/actual-or-estimated-wind-and-solar-power-generation).This airflow dag runs every 30 minutes interval.

## Pre-requisites
1. A Postgres database as the destination

## DEV SETUP
1. Requirements
    - python installed
    - pre-commit installed
    - ruff installed
    - mypy installed
    - pytest installed

## DEVELOPMENT
1. Clone the repo.
2. rename `.env-example` to `.env`
2. Change the value of variables in `.emv` according to your requirements.
3. Browse: `http://localhost:8080` to access the airflow UI.

## Testing
It is recommended to perform unit test before commiting the code. To run unit test, run the following command

`pytest`

The test contains the following:
1. Integrity test on the Dag
2. Unit test on the Dag tasks
3. Unit test on every relevant function


## Type Checking and Linting
This repo uses `pre-commit` hooks to check type and linting before committing the code.

Perform below commands to:
1. Type Checking
`mypy .`
2. Linting
`ruff check .`

