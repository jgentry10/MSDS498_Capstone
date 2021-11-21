# MSDS 498 Capstone Project

## Assignment
- Create a customized Docker container from the current version of Python that deploys a python application.
- Push image to DockerHub or Amazon ECR or Google Container Registry.
- Pull image down and run it on a cloud platform cloud shell:  Google Cloud Shell or AWS Cloud9.
- Deploy an application to managed Kubernetes cluster.
<br />

## Project Overview
In order to complete the project, the following technologies were deployed on to a newly created VM hosted within Google Cloud.
<br />
  - Flask: Used to create a REST API around the model.
  - Docker: Used to ensure code runs in any environment with Docker.
  - Kubernetes: Used to automate the scaling of the serving layer.

<br />
Within Google Cloud, I'll follow these steps to deploy the application to a Kubernates cluster. 
<br />

![Architecture Diagram](MSDS_498_P1_JPG_Diagram.png)

<br />
Step 1: Create a VM instance.
<br />
Step 2: Prepare the VM instance. Install all the necessary software and add the required files to it.
<br />
Step 3: Train the ML model. Build and run a Docker container to train the model and output a pickle file with the model characteristics.
<br />
Step 4: Upload the pickle file into a bucket of the Google Cloud Storage for loading it later in the prediction model.
<br />
Step 5: Build the prediction model app. Use the prediction model wrapped in a Flask API, requirements, and Dockerfile to build the Docker container. Then, run a Docker container that loads the pickle file from the Google Cloud Storage, waits for the client POST request, and gives the prediction results.
<br />
Step 6: Run the prediction model container image with Kubernetes and make it accessible publicly via a global URL.
<br />
Step 7: Sent a POST request to the global URL and receive the predictions.
<br />


