# docker-postgres-pgadmin

Create a postgresql-pgadmin container

## Instructions

1. Create permanent volume route:

    sudo mkdir /opt/postgresql/data


2. Run docker compose:

    docker compose up


3. Access pgadmin in browser:

    https://localhost:5050


## Data

*User pgadmin*: admin@admin.com

*Password pgadmin*: admin


### Connection to DB

*Connect*: postgres container    (sugestion, could be anything)

*database*: postgres

*user*: postgres

*passsword*: postgres
