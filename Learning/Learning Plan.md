Learning plan to advancing my data engineer career, currently i have listed skills and tool required for a DE III as per job postings online. The self decided timeline is 2 Years from my pivot that is 21 months from the time of writing this.

## Foundational Concepts

### Data Processing:

- Distributed Computing
  - **Start Date:**
  - **End Date:**
  - **Description:** Distributed computing frameworks like Apache Spark or Dask are essential for processing large volumes of data efficiently in parallel across multiple nodes. Understanding distributed computing principles will enable you to design and optimize data processing pipelines for performance and scalability.
  - **Suggestions:** 
    - Gain hands-on experience with Apache Spark through online tutorials or courses.
    - Experiment with Dask for parallel computing in Python.

- Stream Processing
  - **Start Date:**
  - **End Date:**
  - **Description:** Stream processing frameworks enable real-time processing of streaming data with low latency and high throughput.
  - **Suggestions:** 
    - Learn about stream processing concepts and use cases.
    - Explore stream processing frameworks such as Apache Kafka, Apache Flink, or Apache Storm.

- Batch Processing
  - **Start Date:**
  - **End Date:**
  - **Description:** Batch processing frameworks like Apache Hadoop or Apache Beam are used for processing large volumes of data in batches. Understanding batch processing concepts will be essential for designing and implementing batch data processing pipelines for analytics and reporting.
  - **Suggestions:** 
    - Learn MapReduce programming for batch processing in Hadoop.
    - Explore Apache Beam for building unified batch and stream processing pipelines.

## Data Engineering Tools

### Workflow Automation:
- [[Airflow]]
  - **Start Date:**
  - **End Date:**
  - **Description:** Airflow is a powerful open-source platform for orchestrating complex workflows and data pipelines. It allows you to schedule, monitor, and manage workflows programmatically, making it a valuable tool for data engineers.
  - **Suggestions:** 
    - Dive into Airflow's documentation and tutorials to understand its core concepts.
    - Experiment with building and scheduling data pipelines using Airflow.

- DBT Orchestration on Airflow
  - **Start Date:**
  - **End Date:**
  - **Description:** DBT (Data Build Tool) is a popular tool for transforming and modeling data in data warehouses. Integrating DBT with Airflow allows for automated orchestration of DBT jobs, enabling efficient and scalable data pipeline management.
  - **Suggestions:** 
    - Learn how to integrate DBT with Airflow for orchestrating data transformations.
    - Explore DBT's documentation and community resources for best practices.

- Github Actions for CI/CD
  - **Start Date:**
  - **End Date:**
  - **Description:** GitHub Actions provides a flexible framework for automating software development workflows, including continuous integration and continuous deployment (CI/CD). Learning how to use GitHub Actions will streamline your development process and improve productivity.
  - **Suggestions:** 
    - Set up CI/CD workflows for your data projects using GitHub Actions.
    - Explore GitHub Actions marketplace for pre-built workflows and actions.

### Containerisation and Orchestration:
- [[Docker]]
  - **Start Date:** 12/04/2024
  - **End Date:** 14/04/2024
  - **Description:** Docker is a containerisation platform that simplifies the process of packaging, deploying, and managing applications. Understanding Docker will enable you to create portable and reproducible environments for your data engineering projects.
  - **Suggestions:** 
    - Learn Docker basics such as container creation, Dockerfile, and Docker Compose.
    - Explore Docker's networking and storage options for data-intensive applications.
  - **Comments:** Main objective is to learn for Airflow. Docker is pretty straightforward. You need configuration for every application that is required and compose it in a single file. The format can be learned, but it's widely used with a big community, so no need to learn how to write it myself for now.

- Kubernetes
  - **Start Date:**
  - **End Date:**
  - **Description:** Kubernetes is an open-source container orchestration platform for automating deployment, scaling, and management of containerised applications. Learning Kubernetes will be valuable for deploying and managing containerized data applications at scale.
  - **Suggestions:** 
    - Set up a Kubernetes cluster locally using Minikube or kind.
    - Experiment with deploying and managing data-intensive applications on Kubernetes.

## Programming Languages

### Scripting and Data Manipulation:
- Python
  - **Start Date:**
  - **End Date:**
  - **Description:** Python is a versatile programming language widely used in the data engineering field for data manipulation, analysis, and pipeline orchestration. Mastering Python will enable you to write efficient and scalable data processing code.
  - **Suggestions:** 
    - Practice Python programming with data manipulation libraries like Pandas and NumPy.
    - Explore Python frameworks like Flask for building REST APIs for data services.

- Jinja
  - **Start Date:**
  - **End Date:**
  - **Description:** Jinja is a templating language commonly used for generating dynamic content in Python web applications and data pipelines. Learning Jinja will enable you to create dynamic templates for generating reports, emails, or configuration files.
  - **Suggestions:** 
    - Dive into Jinja's documentation and learn its templating syntax and features.
    - Experiment with integrating Jinja templates into your data processing pipelines.

### Functional and Big Data Processing:
- Scala
  - **Start Date:**
  - **End Date:**
  - **Description:** Scala is commonly used in the Apache Spark ecosystem for writing scalable and performant data processing applications. Learning Scala will be valuable for building high-performance data processing pipelines.
  - **Suggestions:** 
    - Learn Scala basics and functional programming concepts.
    - Explore Scala's ecosystem for big data processing, including Spark and Akka.

- Java
  - **Start Date:**
  - **End Date:**
  - **Description:** Java is widely used for building enterprise-grade data processing applications and frameworks. Understanding Java will be valuable for contributing to and extending existing data processing tools and libraries.
  - **Suggestions:** 
    - Practice Java programming with a focus on data processing libraries and frameworks.
    - Explore Java ecosystem tools like Hadoop and Flink for big data processing.

- Go
  - **Start Date:**
  - **End Date:**
  - **Description:** Go (Golang) is gaining popularity in the data engineering community for building high-performance and concurrent data processing applications. Learning Go will enable you to leverage its performance and concurrency features for data processing tasks.
  - **Suggestions:** 
    - Learn Go programming fundamentals and concurrency patterns.
    - Experiment with building data processing applications using Go's standard library and third-party packages.

## Additional Focus Areas

### Data Storage & Management:
- NoSQL
  - **Start Date:**
  - **End Date:**
  - **Description:** NoSQL databases like MongoDB or Cassandra are commonly used for storing and managing unstructured or semi-structured data. Understanding NoSQL databases will be valuable for designing and optimizing data storage solutions for diverse data types.
  - **Suggestions:** 
    - Gain hands-on experience with NoSQL databases through tutorials or online courses.
    - Explore data modeling techniques and best practices for NoSQL databases.

### Data Infrastructure:
- Data Lakes
  - **Start Date:**
  - **End Date:**
  - **Description:** Data lakes are central to modern data architectures, providing scalable storage for diverse data types including structured, semi-structured, and unstructured data. Understanding data lake concepts and technologies like Apache Hadoop or AWS S3 will be essential for building scalable and cost-effective data platforms.
  - **Suggestions:** 
    - Set up a data lake environment using Hadoop or cloud-based services like AWS S3.
    - Explore data lake architectures and best practices for data organization and governance.

### Data Quality & Governance:
- Data Quality and Governance
  - **Start Date:**
  - **End Date:**
  - **Description:** Data quality and governance are critical aspects of any data-driven organization. Understanding data quality assessment techniques, data governance frameworks, and regulatory compliance requirements will be essential for ensuring data integrity and regulatory compliance.
  - **Suggestions:** 
    - Learn about data quality assessment techniques and tools.
    - Explore data governance frameworks such as DAMA-DMBOK and COBIT for establishing data governance practices.

### Data Streaming:
- Kafka
  - **Start Date:**
  - **End Date:**
  - **Description:** Apache Kafka is a distributed streaming platform used for building real-time data pipelines and event-driven architectures. Mastering Kafka will enable you to design and implement scalable and fault-tolerant streaming data applications.
  - **Suggestions:** 
    - Set up a Kafka cluster locally and experiment with building real-time data pipelines.
    - Explore Kafka ecosystem tools like Kafka Connect and Kafka Streams for building end-to-end streaming applications.
