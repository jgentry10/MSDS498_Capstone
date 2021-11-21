# MSDS 498 Capstone Project

<br />

## Project Overview

<br />

In order to complete the project, we will use the following technologies deployed on to a VM hosted within Google Cloud.

<br />

  - Flask: a micro-web framework, known for its lightweight and simplicity. We will use it to create a REST API around our model.

<br />

  - Docker: The most popular containerization technology out there. We will use it to ensure our code runs in any environment with Docker.

<br />

  - Kubernetes: The most widely adopted container orchestration technology. We will use it to automate the scaling of our serving layer.

<br />

Also, we needed to pick a cloud vendor to show you the example end to end, so we just went with GCP (Google Cloud Platform). However, you can easily replicate this example in any cloud platform, since Kubernetes is offered as a service by all major cloud providers.
To go from training to serving our model, we set up the following system architecture using the technologies mentioned above. We also labeled the components chronologically and described them in more detail to walk through the diagram.
