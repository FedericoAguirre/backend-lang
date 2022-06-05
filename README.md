# Backend language

Este projecto es el análisis de un tweet que preguntaba cuál sería el primer lenguaje de su elección para aprender a programar backend.

El análisis se hizo utilizando un notebook de [Apache Zeppelin](https://zeppelin.apache.org/) y [Apache Spark](https://spark.apache.org/).

## Docker Apache Zeppelin.

Ejecuten el siguiente comando en la raíz para habilitar el entorno de trabajo:

```bash
docker run -u $(id -u) -p 8080:8080 --rm -v $PWD/logs:/logs\
    -v $PWD/notebook:/notebook -v $PWD/data:/data \
	-e ZEPPELIN_LOG_DIR='/logs' -e ZEPPELIN_NOTEBOOK_DIR='/notebook' \
    --name zeppelin apache/zeppelin:0.10.0
```

Accedan al url de [Zeppelin local](http://localhost:8080).

Abran el notebook **backend-lang**.
