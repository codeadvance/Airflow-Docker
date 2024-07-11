airflow
#This is the python script where it activates airflow. First off

using Apache Airflow with Docker, including installation and creating a DAG (Directed Acyclic Graph) file.

Step 1: Install Docker Download Docker:

For Windows/Mac: Download Docker Desktop from here and follow the installation instructions. For Linux: Follow the instructions here. Install Docker: https://hub.docker.com/

Windows/Mac: Run the downloaded installer and follow the setup steps. Ensure Docker Desktop is running. Linux: Use the terminal commands from the Docker installation page to set up Docker. Verify Installation:

Open a terminal (or command prompt on Windows) and run: sh Copy code docker --version You should see the Docker version information if the installation was successful. Step 2: Set Up Apache Airflow with Docker Pull the Apache Airflow Docker Image:

Open a terminal and run: sh

Then download the welcome.py and docker-composer.yaml Make sure you open these files in Visual Studio Code and run the docker-composer.yaml by right click the file name on the right bar and click compose up or type docker composer up in the terminal.

This will start running the airflow

Then you create a new folder called DAGS in Airflow-Docker and save Welcome_dag.py in the folder.

The containers that you created in DAG file will show in Airflow application.

Once you are done airflow- right click compose down or type docker compose down 
