# reto-data_dd360
## Estructura del proyecto

Estos son los archivos y directorios más relevantes del proyecto:
```
.
├── docker #Python dependencies
    ├── airflow
        ├── Dockerfile
        ├── requirements.txt
        ├── start-airflow.sh
    ├── docs
        ├── queries_snowflake.sql # queries ejecutadas en snowflake
    postgres
        ├── Dockerfile
        ├── init-hive-db.txt
├──mnt
    ├── airflow
        ├── dags/ # contiene los dags y puede organizar sus DAG en subcarpetas 
├── .env
├── docker-compose
```
# Comenzando

## Requisitos de instalación

- [Docker](https://docs.docker.com/install/) `2.1.0.1` or greater.

## Iniciado Airflow 
```
inicar airflow docker-compose up -d   
parar airflow docker-compose stop
reiniciar airflow docker-compose restart
```

## Acceder a la interfaz web

Una vez que construya y ejecute Airflow, abra un navegador web y navegue a [http://localhost:8080](http://localhost:8080).
Utilice las siguientes credenciales predeterminadas para iniciar sesión:

> usuario: airflow  
> Contraseña: airflow

Una vez iniciada la sesión, accederá a la interfaz principal de Airflow.

## Se deben crear dos Conexiones para que funcione el flujo 
```
Conexión a snowflake 
```
https://drive.google.com/drive/u/0/folders/17aT4fiNMFErh1VX1u9J6mv09mbJocOqI
