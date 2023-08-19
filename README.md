# docker-postgres-pgadmin

Create a postgresql-pgadmin container

## Notes

This docker compose run inside a network with address 192.168.101.0/24.
If you want to change this address, you need to change the network address in docker-compose.yml.

## Instructions

1. Create permanent volumes routes:

    ```bash
    sudo mkdir /opt/pgsql/data
    sudo mkdir /opt/pgadmin/data
    ```

2. Run docker compose:

    ```bash
    docker compose up -d
    ```

3. Access pgadmin in browser:

    ```bash
    https://localhost:5050
    ```

4. Stop docker compose:

    ```bash
    docker compose down
    ```

## Data

*User pgadmin*: <admin@admin.com>

*Password pgadmin*: admin

### Connection to DB

*Connect*: postgres container    (suggestion, could be anything)

*database*: postgres

*user*: postgres

*passsword*: postgres
