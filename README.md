# PostgreSQL-PostGIS-TimescaleDB

PostgreSQL + PostGIS + TimescaleDB ready-to-use docker image 🐘🌎📈

Docker image with:
* [PostgreSQL](https://www.postgresql.org/) 
* [PostGIS](http://postgis.net/)
* [TimescaleDB](https://www.timescale.com/)

Current versions of components:
* PostgreSQL: **10.1** ([Source docker image](https://store.docker.com/images/postgres))
* PostGIS: **2.4.2** ([Release archive](https://github.com/postgis/postgis/releases/tag/2.4.2))
* TimescaleDB: **0.7.1** ([Release archive](https://github.com/timescale/timescaledb/releases/tag/0.7.1))

How to build:

```bash
$ docker build -t binakot/postgres-postgis-timescaledb .
```

How to run:

```bash
$ docker run -d --name postgres -e POSTGRES_PASSWORD=postgres binakot/postgres-postgis-timescaledb
```

Fast start with docker stack:

```bash
$ docker stack deploy -c stack.yml postgres
```
