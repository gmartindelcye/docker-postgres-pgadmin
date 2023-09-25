# docker-postgres-pgadmin

Create a postgresql-pgadmin container

## Notes

This docker compose run inside a network with address 192.168.101.0/24.
If you want to change this address, you need to change the network address in docker-compose.yml.

## Instructions

1. Create permanent volumes routes:

    ```bash
    sudo mkdir -p pgsql/data
    sudo mkdir -p pgadmin/data
    ```

2. Change permissions to pgadmin directory in order to be accessed:

    ```bash
    sudo chown -R 5050:5050 pgadmin
    ```

3. Run docker compose:

    ```bash
    docker compose up -d
    ```

4. Access pgadmin in browser:

    ```bash
    https://localhost:5050
    ```

    or

   ```bash
   https://server_url:5050
   ```

5. Stop docker compose:

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

*password*: postgres
