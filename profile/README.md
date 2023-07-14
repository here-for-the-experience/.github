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
  + https://dev.redevops.store
  + https://dev.admin.redevops.store
### Dev Environment :
#### Backend :
  + https://dev.api.redevops.store
  + http://dev.auth.redevops.store
### 

### Frontend :
  + https://redevops.store
  + https://admin.redevops.store

### ArgoCD :

  For Dev environment :
  + url : https://dev.argocd.redevops.store/
  + username : admin
  + password : VoQtVcGMkQAwIZGI
  For Production environment :
  + url : https://argocd.redevops.store/
  + username : admin
  + password : EgNBAzTkR64OIKYS

### Monitoring with Grafana :
    url : https://grafana.redevops.store/
    username : admin
    password : prom-operator


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
### Github Strategy

Our GitHub strategy focuses on ensuring effective collaboration, security, and access control within our organization. Here are the key components of our strategy:

##### Repository Organization

###### Logical Segmentation: 
We organize repositories based on logical boundaries, ensuring that each repository contains related code and resources. This promotes clarity, ease of navigation, and focused ownership of specific components.

###### Granular Access Control: 
We implement granular access control at the repository level. Access permissions are assigned based on role and responsibility, ensuring that team members have appropriate access to repositories they need for their work.

###### Collaboration and Ownership: 
Each repository has defined owners or maintainers responsible for code review, merging pull requests, and managing overall repository health.

##### Branching and Version Control
###### Branching Model: 
We adopt a branching model, such as GitFlow or a similar strategy, to manage feature development, bug fixes, and releases. This model ensures a structured and organized approach to version control and release management.

###### Pull Requests and Code Review:
All changes are made via pull requests, enabling thorough code review by designated reviewers.

##### Security and Compliance
###### Secure Coding Practices: 
We follow secure coding practices and guidelines to minimize vulnerabilities and maintain a secure codebase. This includes adhering to best practices for input validation, authentication, authorization, and handling sensitive data.

###### Code Analysis and Testing: 
We incorporate static code analysis tools and automated testing frameworks into our development process.

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

A snapshop of SonarQube used in our application :

![image](https://github.com/here-for-the-experience/.github/assets/77661612/f6024793-e6dd-451c-92c8-61e2198ac622)


## ArgoCD

We have chosen ArgoCD for its capabilities as a GitOps continuous delivery tool. By leveraging ArgoCD, we can automate the deployment process of our application and ensure consistent and reliable deployments to our Kubernetes clusters. ArgoCD allows us to declaratively define our desired application state using Git repositories, enabling us to track changes, roll back to previous versions if needed, and easily manage application deployments through its intuitive web interface and CLI.


A snapshop of ArgoCD used in our application :

![image](https://github.com/here-for-the-experience/.github/assets/77661612/6fa624c5-5c4e-41af-8c6b-b7fb0b351436)


## Canary Release for Production

We have incorporated the Canary Release strategy into our deployment process to ensure a smooth and controlled rollout of new features and updates. Canary Release is a technique that involves releasing a new version of the application to a small subset of users or production environment before making it available to the entire user base. Here's why we have chosen to use the Canary Release strategy and how it helps us:

  + Controlled Rollout and Risk Mitigation
  + Early Feedback and Validation
  + Performance and Scalability Testing
  + Incremental Deployment and Rollback Capability
  + Continuous Improvement and Learning

A snapshop of Canary Release used in our application :



## Grafana

Grafana was selected for its powerful data visualization and monitoring features. With Grafana, we can create interactive dashboards and graphs to visualize real-time metrics, time series data, and logs from various sources within our application. By monitoring these metrics and setting up alerts, we can gain deep insights into the performance and health of our system, enabling us to proactively identify issues and take necessary actions to ensure optimal application performance.

A snapshop of Grafana used in our application :

![image](https://github.com/here-for-the-experience/.github/assets/77661612/9cc9ebb3-2c7c-479f-90b7-c3b5cc4dc3d8)


A snapshop of Argo Rollouts used in our application :
## Argo Rollouts
We have incorporated Argo Rollouts into our deployment process to facilitate advanced deployment strategies and enhance the overall reliability and resilience of our application. Argo Rollouts builds upon the capabilities of ArgoCD, our chosen continuous delivery tool, and provides additional features specifically designed for managing complex deployment scenarios.


<img width="1440" alt="image (1)" src="https://github.com/here-for-the-experience/.github/assets/77661612/6d194d4e-89f2-4ffb-90eb-dee5ecd1da9d">

## Provisioning EKS Clusters and Resources in Multiple Environments with Terragrunt(A Thin Wrapper of Terraform) 

We have incorporated Terragrunt into our project to enhance the management and orchestration of our Terraform deployments.Terragrunt simplifies the management of remote state in Terraform deployments. With Terragrunt, we can define and configure remote state backends. Terragrunt promotes code reusability and composition by allowing us to define reusable Terraform modules and configurations. Terragrunt supports environment-specific configuration, allowing us to define environment-specific variables and settings for our Terraform deployments.


## Reporting Problems 
You can send us a mail at :
+ iam.reduan@gmail.com
+ Raufun.nazin13@gmail.com
+ shakil.csedu@gmail.com

## Contributors 
+ Alve Reduan
+ Raufun Nazin Srizon
+ Fahim Shakil
