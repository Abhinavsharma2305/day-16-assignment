# PySpark RDD Employee Data Processing
## Project Description
This project uses PySpark RDDs to process an employee dataset. The application performs the following operations:
Reads employee data from a CSV file.
Sorts employees by salary in descending order.
Calculates the total salary for each department.
Identifies the top 3 highest-paid employees and saves the output to a file.
The project is containerized using Docker, which installs Java, Python, and Apache Spark and automatically runs the PySpark application.
## Project Structure
Assignment 16/
pyspark_app.py
employee.csv
output.txt
requirements.txt
Dockerfile
README.md
## Employee Dataset
csv
id,name,department,salary
1,Amit,IT,55000
2,Rahul,HR,40000
3,Neha,IT,65000
4,Priya,Finance,70000
5,Karan,IT,50000
6,Simran,HR,45000
7,Rohit,Finance,60000
## Requirements
- Docker
## Build Docker Image
bash
docker build -t employee-rdd .
## Run Docker Container
docker run --rm employee-rdd
## Output
Employees sorted by salary (displayed on the console)
Department-wise total salary (displayed on the console)
Top 3 highest-paid employees saved in `output.txt`
## Technologies Used
Python 3.12
PySpark 3.5.6
Apache Spark
Docker
