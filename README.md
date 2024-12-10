# streamlitUI-app

Project: StreamlitUI Application

Description:
This project is a simple Python application which features simple chatbot created using OpenAI and StreamlitUI. This application can be deployed as a Docker container and deployed to a Kubernetes cluster

Prerequisites:

Docker
Kubernetes
Python 3.11
Installation:

Running Locally:
Clone this repository.
Set up your Python development environment.

$ pip install streamlit

Validate the installation by running our Hello app:
$ streamlit hello

You can open browser at http://localhost:8502/ to view your deployment

To get OPEN_API_KEY-
To generate an OpenAI API key, tap on your name to view the dropdown menu. Click the 'View API keys' option. At this stage, you'll see a window with the option 'Create new secret key' near the center.

Replace the key with your newly created key

Build the Docker image:
$ docker build -t my-app .

Run the Docker container:
$ docker run -it -p 5000:5000 my-app

Access the application in your browser at http://localhost:5000.
Deployment to Kubernetes:

Build the Docker image.
Apply the deployment.yaml and service.yaml files to your Kubernetes cluster.
Access the application through the Kubernetes service's IP address and port.
Additional Notes:

You can customize the Dockerfile and YAML files to fit your specific needs.
Consider using a configuration management tool like Ansible or Puppet to automate the deployment process.
Implement proper logging and monitoring for your application.
Secure your application by following best practices for Docker and Kubernetes security.
