# Microservice with Kubernetes

This project showcases the deployment of a microservice using Kubernetes. It utilizes Helm charts for easier management and deployment of the microservice.

## Project Structure

The project consists of the following components:

- `config.yaml`: This file contains the deployment and service configurations for the microservice. It is used when deploying the microservice without Helm.
- `charts/`: This directory contains the Helm charts used to deploy the microservice. It includes the necessary configurations and templates for deploying the microservice in a Kubernetes cluster.
- `values/`: This directory contains the Helm charts value used to deploy the different microservice. 
- `helmfile.yaml/`: This file contains the Helm charts releases the different microservice.
- Other project files: These files are used by the Helm chart to deploy the microservice and may include values, templates, or additional configurations.

## Deployment

To deploy the microservice, you can use Helm by following these steps:

1. Install Helm on your local machine and set up a Kubernetes cluster.
2. Navigate to the project's root directory.
3. Customize the Helm chart configurations in the `values.yaml` file or any other relevant files, if needed.
4. Run the following command to deploy the microservice using Helm:

   ```shell
   helmfile sync```
5. Verify that the microservice is successfully deployed by checking the resources created in your Kubernetes cluster.

Alternatively, if you prefer to deploy the microservice without Helm, you can use the config.yaml file directly. Refer to your Kubernetes documentation or tools to apply the configuration and create the necessary resources.

##Additional Information
Feel free to explore and modify the project according to your requirements. You can add more microservices, customize the Helm charts, or integrate other Kubernetes features to enhance the deployment.

