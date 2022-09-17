# Pexon certifcation portal

## Challenge Description:

A Python Flask-based web app has been created to provide a portal through which Pexon employees can provide their Name, Certification(s) titles, and upload corresponding certification files in pdf, png and jpeg file formats. 

The web app allows the upload, and storage of these employee credentials onto the backend sqlite database. 

Registered credentials and corresponding uploader details are further presented in a table, and a download link is provided for each entry in order to allow user to download and view the employees certifications and credentials. 

## Route unit tests 

The app contains 3 routes that can be tested for:
- GET /
- POST /upload
- GET /cert/{id} 

For demonstration purposes, a 'tests' folder is created, consisting of a python file 'test_routes.py' which in turn consists of a script to test for the 2nd route i.e. the /upload route.

In order to carry out the test one should run command:
```
PYTHONPATH=. pytest
```
Furthermore within the 'tests' folder, the writer of the app has included his own 
recently acquired AWS Certified Cloud Practitioner.pdf certification that can be 
used to run a manual upload test on the app.

Due to time constraints further testing was not done. However more route test should be carried out. It would be recommended to do the following route tests:

- 



## Requirements / Setup Environment

python 
flask 

## Run Project
commands for run project 
python3 main.py


## Run as docker container

Please use the dockerfile provided in order to make a docker image (using docker build command) containing the python script (main.py), and the docker run command in order run a docker container with this image containing the app python script . 

Note: For this, the following os and dependancies will be required: 

- python alpine3.6 image 
- pysqlite3
- flask

## Docker compose 

The Docker container can also be run using the Docker compose file.
Please use the docker-compose.yml file which is a yaml file describing Docker container configuration. Using the docker-compose up command in the same folder as the file, the Docker container can be run.


