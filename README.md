# Docker Zeppelin

This repository contains [Apache Zeppelin](https://zeppelin.apache.org/) docker image, which is tuned to work with BDE clusters.

# Example Usage

For example usage see [docker-compose.yml](./docker-compose.yml) and [SANSA-Notebooks repository](https://github.com/SANSA-Stack/SANSA-Notebooks).

# Dev
```
Build Zeppelin:
```
make build
```

Start Hadoop/Spark cluster with Zeppelin notebook:
```
make up
```


Start Hadoop/Spark cluster with Zeppelin notebook running with --detach:
```
make upd
```

Tear down Hadoop/Spark cluster with Zeppelin notebook:
```
make down
```

Bash into Zeppelin container:
```
make bash
```

Build and run Zeppelin separately:
```
make up
docker stop dockerzeppelin_zeppelin_1 && docker rm dockerzeppelin_zeppelin_1
make run

For more details see the Makefile.
