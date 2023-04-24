# sunrise-nyc-data

This repository houses the data stack for Sunrise NYC.


## features

## installation

- set up python3.10 venv with pip-tools
- pip-sync from requirements.txt
- place slack api token in the meltano/.env
- docker run postgres container
  docker run -p 5432:5432 -e POSTGRES_USER=meltano -e POSTGRES_PASSWORD=password -d postgres
- make sure that the target-postgres settings match up with the user/pass set
- give it a few seconds to start up
- cd meltano
  meltano run tap-slack target-postgres


## usage

## todo

- Determine licensing: which and how
- set up docker compose to:
  - spin up postgres container
  - run meltano elt
