# SQLAlchemy Object Relational Tutorial
## Here I am studying how to implement the correct way sqlAlchemy, doing the tutorial accessible here: https://docs.sqlalchemy.org/en/13/orm/tutorial.html


## How to run:

## Docker
### ---- Postgres
sudo docker run \
    --name postgres \
    -e POSTGRES_USER=vsantos93 \
    -e POSTGRES_PASSWORD=swordfish \
    -e POSTGRES_DB=teste \
    -p 5432:5432 \
    -d \
    postgres

### ---- Adminer
sudo docker run \
    --name adminer \
    -p 8080:8080 \
    --link postgres:postgres \
    -d \
    adminer

 `Using postgres and adminer, we can see our database by accessing:
http://localhost:8080/`