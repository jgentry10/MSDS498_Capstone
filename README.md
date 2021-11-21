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
  - Flask: a micro-web framework, known for its lightweight and simplicity. We will use it to create a REST API around our model.
  - Docker: The most popular containerization technology out there. We will use it to ensure our code runs in any environment with Docker.
  - Kubernetes: The most widely adopted container orchestration technology. We will use it to automate the scaling of our serving layer.

<br />

Also, we needed to pick a cloud vendor to show you the example end to end, so we just went with GCP (Google Cloud Platform). However, you can easily replicate this example in any cloud platform, since Kubernetes is offered as a service by all major cloud providers.
To go from training to serving our model, we set up the following system architecture using the technologies mentioned above. We also labeled the components chronologically and described them in more detail to walk through the diagram.
