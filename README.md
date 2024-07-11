# Automating Data Scraping with Apache Airflow
## Introduction:
Harness the power of Apache Airflow to automate web scraping of raw data from LinkedIn and Indeed, storing it seamlessly in an Amazon S3 bucket. This guide walks you through using Docker to install and configure Airflow, creating a Directed Acyclic Graph (DAG) to manage your scraping workflow, and ensuring your data is securely saved in the cloud.

## Step-by-Step Guide:
Step 1: Install Docker
Download Docker:

Windows/Mac: Download Docker Desktop from the Docker website and follow the installation instructions.
Linux: Follow the installation instructions provided here.
Install Docker:

Windows/Mac: Run the downloaded installer and complete the setup. Ensure Docker Desktop is running.
Linux: Use terminal commands from the Docker installation page to set up Docker.
Verify Installation:

Open a terminal or command prompt and run:
sh
Copy code
docker --version
You should see the Docker version information if the installation was successful.
Step 2: Set Up Apache Airflow with Docker
Pull the Apache Airflow Docker Image:

Open a terminal and run:
sh
Copy code
docker pull apache/airflow
Download and Configure Files:

Download welcome.py and docker-compose.yaml.
Open these files in Visual Studio Code.
Run Docker Compose:

Right-click docker-compose.yaml in Visual Studio Code and select Compose Up, or run the following command in the terminal:
sh
Copy code
docker-compose up
This will start running Airflow.
Create a DAG for Web Scraping:

Create a new folder named DAGS in the Airflow-Docker directory.
Save Welcome_dag.py in the DAGS folder.
View DAG in Airflow:

The containers created in the DAG file will be visible in the Airflow application.
Step 3: Storing Data in Amazon S3
Configure your DAG to scrape data from LinkedIn and Indeed.

Use Python scripts within the DAG to save the scraped data to an Amazon S3 bucket.

Shut Down Airflow:

The screenshot of Docker: 

<img width="956" alt="image" src="https://github.com/user-attachments/assets/2c7be1ab-59fd-4f50-81cf-b82470d5a539">


When finished, right-click docker-compose.yaml and select Compose Down, or run:
sh
Copy code
docker-compose down
This setup ensures your data scraping process is automated, efficient, and scalable, with data securely stored in Amazon S3 for further analysis and use.

The screenshot of scraping job source:

<img width="944" alt="image" src="https://github.com/user-attachments/assets/631494bd-5f05-4ca2-9e08-809dcd63a40a">

