# Automated CI/CD Pipeline for Docker Containers on AWS ECS Using Jenkins
## Description

This project automates the entire Continuous Integration and Deployment (CI/CD) pipeline for Docker containers on AWS ECS, utilizing Jenkins. The pipeline streamlines code fetching, Docker image building, code analysis, image upload to Amazon ECR, and deployment to ECS. Slack notifications ensure real-time alerts about deployment status, optimizing the development workflow.

## Technologies

- CI/CD Orchestration: Jenkins
- Containerization: Docker
- Code Quality Analysis: SonarQube
- Artifact Management: Amazon ECR
- Deployment: AWS ECS (Elastic Container Service)
- Notifications: Slack
   
## Architecture Overview

- Jenkins CI Server: Hosted on an EC2 instance, Jenkins automates the pipeline, fetching code, running builds, tests, and quality 
  analysis.
- Docker Containerization: Jenkins builds and tests Docker images, pushing them to Amazon ECR for storage.
- SonarQube: Integrated with Jenkins to perform static code analysis and enforce quality standards.
- AWS ECS: After a successful build, Jenkins updates ECS services to deploy the new Docker containers by pulling images from ECR.
- Slack Integration: Notifications inform the team of deployment and build status changes.
- AWS Infrastructure: Utilizes EC2, ECS, and ECR services for seamless CI/CD orchestration and scalability.
  
  

## Walk-through:
