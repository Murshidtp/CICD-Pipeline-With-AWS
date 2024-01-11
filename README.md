# Continuous Integration and Continuous Deployment (CI/CD) Pipeline With AWS Services

## Overview

This project showcases an end-to-end CI/CD pipeline implementation using AWS services. The pipeline incorporates AWS CodeCommit for version control, AWS CodeBuild for automated build processes, AWS CodeDeploy for deployment automation, and AWS CodePipeline for orchestrating the entire workflow. Additionally, the Amazon Elastic Container Registry (ECR) is utilized for storing Docker images. The primary goals of this pipeline are to improve development efficiency, reduce time by automating repetitive tasks, and minimize manual interventions.

## AWS Services Used

1. **AWS CodeCommit:**
   - Used for version control, storing and managing source code securely.

2. **AWS CodeBuild:**
   - Automates the build and packaging processes of the application.

3. **AWS CodeDeploy:**
   - Automates deployment processes, ensuring consistent and reliable application releases.

4. **AWS CodePipeline:**
   - Orchestrates the entire CI/CD workflow, integrating CodeCommit, CodeBuild, and CodeDeploy seamlessly.

5. **Amazon ECR (Elastic Container Registry):**
   - Used to store and manage Docker container images securely.

## Project Structure

- The source code is hosted in AWS CodeCommit repositories.
- AWS CodeBuild is configured to automatically build the application on code changes.
- The resulting artifacts are stored in Amazon ECR as Docker images.
- AWS CodeDeploy automates the deployment of the application to the target environment.
- AWS CodePipeline coordinates the entire workflow, triggering the pipeline on code changes.


## Prerequisites

Ensure you have the following set up:

- AWS account with necessary permissions.
- AWS CLI configured with access to CodeCommit, CodeBuild, CodeDeploy, CodePipeline, and ECR.
- `buildspec.yml`: Configuration file for AWS CodeBuild, defining the build steps and environment settings.
- `appspec.yml`: Configuration file for AWS CodeDeploy, specifying how to deploy the application onto the target environment.

## Setup

1. Clone this repository:

    ```bash
    git clone https://github.com/Murshidtp/CICD-Pipeline-With-AWS.git
    cd CICD-Pipeline-With-AWS
    ```

2. Set up AWS services:

    - Create CodeCommit repositories for your application.
    - Configure CodeBuild projects.
    - Set up CodeDeploy for deployment.
    - Create a CodePipeline to orchestrate the workflow.

3. Configure Amazon ECR:

    - Set up an ECR registry for storing Docker images.

4. Modify pipeline configurations:

    - Adjust pipeline configurations in CodePipeline to match your application and environment.

## Usage

1. Push changes to the CodeCommit repository.

2. CodePipeline will automatically trigger the workflow based on the source code changes.

3. CodeBuild will build the application using the specifications in `buildspec.yml`.

4. CodeDeploy will deploy the application to the specified environment based on the instructions in `appspec.yml`.

5. Monitor the CodePipeline dashboard for the pipeline execution and results.


## Troubleshooting

If you encounter any issues, refer to the following:

- AWS CodeBuild logs for build-related problems.
- AWS CodeDeploy logs for deployment issues.
- AWS CodePipeline logs for overall pipeline execution.

...

## Reference

For a detailed walkthrough and tutorial on setting up a CI/CD pipeline with Flask application using AWS CodeBuild, CodeDeploy, and CodePipeline, you can refer to the following article:

[CI/CD of Flask Application using AWS CodeBuild, CodeDeploy, and CodePipeline](https://medium.com/@purnimachowrasia/ci-cd-of-flask-application-using-aws-codebuild-codedeploy-and-codepipeline-part-4-97aef0033c09)

...


