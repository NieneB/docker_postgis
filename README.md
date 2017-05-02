# Postgis on Ubuntu in Docker

### Postgis 2.3.2
### PostgreSQL 9.6
### GEOS 3.5.0
### GDAL 1.11.3 

all on Ubuntu 16.04

# How to run?

  export PGDATABASE=DBname
  export PGUSER=DBUsername
  export PGPASSWORD=DBpassword
  export PGPORT=5432
  export PGHOST=localhost 
  
  docker build -t niene/postgis_ubuntu
  
  docker run --name $PGDATABASE -e POSTGRES_DB=$PGDATABASE -e POSTGRES_USER=$PGUSER -e POSTGRES_PASSWORD=$PGPASSWORD -p $PGPORT:5432 -d niene/postgis_ubuntu

