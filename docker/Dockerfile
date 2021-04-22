FROM apache/airflow:1.10.15-python3.8

COPY --chown=$AIRFLOW_UID:$AIRFLOW_GID . /airflow-prometheus-exporter
WORKDIR /airflow-prometheus-exporter
RUN pip install --no-cache-dir -e .

WORKDIR ${AIRFLOW_HOME}
