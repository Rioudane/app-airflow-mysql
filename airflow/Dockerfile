FROM apache/airflow:2.7.1

USER root
RUN apt-get update && \
    apt-get install -y default-mysql-client && \
    rm -rf /var/lib/apt/lists/*

USER airflow
RUN pip install pymysql mysqlclient requests csvkit
