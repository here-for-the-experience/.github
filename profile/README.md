# Project for BUET CSE FEST DevOps Hackathon

## Project Overview

For the hackathon, we have built a vaccination certificate generation application.Our application is designed to streamline the entire certificate generation process, from data input to certificate delivery. We have leveraged DevOps practices to build a secure, scalable, and highly available infrastructure, enabling users to access and verify their vaccination status effortlessly.

By implementing a seamless integration of development and operations, we have achieved an efficient CI/CD pipeline, allowing for rapid development, testing, and deployment. With containerization and orchestration technologies, our application can easily scale to handle increased user demand while maintaining stability and reliability.

## Using the URLs provided below, you can see the live demo of the application :

### Production Environment :
#### Backend :
  + https://api.redevops.store
  + https://auth.redevops.store
#### Frontend :
  + url
  + url
### Dev Environment :
#### Backend :
  + https://dev.api.redevops.store
  + http://dev.auth.redevops.store
### 

### Frontend :
  + url
  + url

### ArgoCD :

### Monitoring with Grafana :



# Installation :
Installation procedure for each section is provided in their respective repositories.

# Usage
To use the Vaccination Certificate Generation project, follow these steps:

+ Visit the application website or launch the application locally.
+ Register an account or log in if you already have one.
+ While registering, we will generate a vaccination certificate for you which will be authorized by an admin. Only after the authorization
  you will be able to generate you vaccination certificate.

Your vaccination certificate will be generated, and you can download or print it for future use.

# Technologies Used :
 + Frontend: NextJs with TypeScript, shadcn ui as a component library and Tailwind CSS for styling.
 + Backend: FastApi
 + Database: PostgreSQL
 + Authentication: JSON Web Tokens (JWT)


# Features

### Continuous Integration/Continuous Deployment (CI / CD) 

We have implemented a robust CI/CD pipeline for both our backend servers (Backend User and Backend Vaccine) as well as our frontend servers. We believe adoption of CI/CD is a key aspect of DevOps practices and has brought numerous benefits to our development and deployment processes.
Such as :

**Automation and Efficiency** : 

CI/CD automates various stages of the development and deployment process, including code compilation, testing, and deployment. By automating these repetitive tasks, we save valuable time and effort. This automation improves overall efficiency, accelerates the software delivery process, and reduces the risk of manual errors.

**Frequent and Continuous Integration** :

With CI/CD, code changes from multiple developers are frequently integrated into a shared repository. This promotes collaboration, helps identify integration issues early on, and ensures that code changes are continually tested and validated.

**Fast and Reliable Deployment** :

By automating the deployment pipeline, we can ensure consistency in the deployment process, reducing the risk of configuration drift and enabling the rapid rollout of changes.

## Static Analysis with SonarQube

We have incorporated SonarQube into our project to ensure code quality and maintainability. SonarQube performs comprehensive code analysis and static code scanning, allowing us to identify and address code quality issues early in the development process. By integrating SonarQube into our CI/CD pipeline, we can automatically analyze our codebase for various metrics such as maintainability, reliability, and security. This helps us maintain a high level of code quality and adhere to best practices, ensuring the overall robustness and stability of our application

## ArgoCD

We have chosen ArgoCD for its capabilities as a GitOps continuous delivery tool. By leveraging ArgoCD, we can automate the deployment process of our application and ensure consistent and reliable deployments to our Kubernetes clusters. ArgoCD allows us to declaratively define our desired application state using Git repositories, enabling us to track changes, roll back to previous versions if needed, and easily manage application deployments through its intuitive web interface and CLI.

## Canary Release for Production
We have incorporated the Canary Release strategy into our deployment process to ensure a smooth and controlled rollout of new features and updates. Canary Release is a technique that involves releasing a new version of the application to a small subset of users or production environment before making it available to the entire user base. Here's why we have chosen to use the Canary Release strategy and how it helps us:

  + Controlled Rollout and Risk Mitigation
  + Early Feedback and Validation
  + Performance and Scalability Testing
  + Incremental Deployment and Rollback Capability
  + Continuous Improvement and Learning

## Grafana

Grafana was selected for its powerful data visualization and monitoring features. With Grafana, we can create interactive dashboards and graphs to visualize real-time metrics, time series data, and logs from various sources within our application. By monitoring these metrics and setting up alerts, we can gain deep insights into the performance and health of our system, enabling us to proactively identify issues and take necessary actions to ensure optimal application performance.




