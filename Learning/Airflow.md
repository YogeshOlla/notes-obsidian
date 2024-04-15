This document provides guidance on setting up and managing Airflow, an open-source tool utilized for developing, scheduling, and monitoring workflows. Airflow is highly versatile, capable of interfacing with multiple applications, and is Python-based, making it the preferred choice for orchestration tasks. However, it is not suitable for use with APIs, CLIs, or infinite processing.

## Resources

- Official Documentation: [Airflow Documentation](https://airflow.apache.org/docs/)
- Airflow in Docker: [Docker Compose Setup](https://airflow.apache.org/docs/apache-airflow/stable/howto/docker-compose/index.html)

## Airflow Setup Process

To set up Airflow, we'll utilize a Docker image hosted on an EC2 instance. Follow these steps:

1. Download the Docker Compose file from the link provided above. This file serves as a template for the Docker image available on the official Airflow website. It's customizable to suit specific requirements.

2. Choose the Local Executor as the current workload is small.

3. Remove the Redis and Celery executor code since they're not required.

4. Create directories for essential items: `mkdir -p ./dags ./logs ./plugins ./config`

5. Initiate the Docker containers by running the following commands:
 
```
docker compose up airflow-init
docker compose up
   ```

- The first command initializes Airflow and creates the admin account.
- The second command starts the remaining Docker images.Done the docker image is up and running and airflow is accessible