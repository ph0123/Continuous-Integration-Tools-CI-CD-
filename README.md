<!---
CI/CD process <img src="CICD.png" width="500" height="300" />
-->


## CI Tools

# Table of Contents
- [Table of Contents](#table-of-contents)
  - [1. Introduction ](#1-introduction-)
  - [2. Self-Hosted ](#2-self-hosted-)
  - [3. Software as a Service (SaaS) ](#3-software-as-a-service-saas-)
  - [4. Cloud Service Providers ](#4-cloud-service-providers-)
  - [5. Codes Repositories ](#5-codes-repositories-)


## 1. Introduction <a name="1"></a>
* Building your CI/CD pipeline
* What you should know:
  * Application Development.
  * Scripting 
  * Source Code Management
  * CI/CD/CD
    * Continuous Integration
      * Developer work locally and commit to a shared repo
      * That code is integrated with other code.
      * The code is tested.
      * Faster than traditional development.
    * Continuous Delivery
      * Partner to continuous integration
      * Allow for building, testing, and delivery with every code change.
      * Testing of part of delivery minimizes bugs.
    * Continuous Deployment
      * Deployment that has done automatically, without human intervention
* Landscape of CI/CD tools and CI/CD tool categories
  * Self-hosted
  * SaaS-based CI/CD tools.
  * Cloud service providers
* The experimental CI/CD pipeline <img src="CICD_Pipeline.PNG" width="500" height="300" />
## 2. Self-Hosted <a name="2"></a>
* Jenkins:
  * Extended functionality with plugins
  * Blue Ocean plugin for pipeline UI
  * Configured in web UI or Jenskinsfile
  * Jenskinsfile is based on Groovy
  * See Ch01/01_01 folder
* Bamboo:
  * Work with Bitbucket
  * Have to pay depended on number of users and plugins.
  * Java format for configuration or web UI.
* TeamCity:
  * Tight integration with JetBrains IDEs
  * Work with other IDEs like Visual Studio
  * Free license with 100 builds and 3 build agents
  * Automatically configure jobs based on project code
  * We can configure it on configuration file or web UI.
  * Config files can be XML or Kotlin format.
* GoCD
  * Free and Open Source CD server.
  * Focus is on pipeline
  * Pipelines are make of stages, jobs, and tasks
  * We can configure it on configuration file or web UI.
  * Config files can be XML
  * Plugin support for JSON and YAML formats
## 3. Software as a Service (SaaS) <a name="3"></a>
* TravisCI
  * Popular choice for opensource projects
  * Works exclusively with GitHub projects
  * Used test pull requests
  * Configured in .travis.yml
  * Starts and connects to services
  * Allows for integration and system testing
  * Can be extended with third party applications, clients, tools, and libraries
* Codeship
  * Basic version: only edit on Web UI, no docker support, shared VMs, ... 
  * Pro version: Both WebUI and configuration file, Docker support built in, Dedicated VMs, ...
* CircleCI
  * Run all OS: linux, windows, macOS
  * Docker is used for running jobs
  * Work with cloud or local services.
  * Command-line for local actions.
## 4. Cloud Service Providers <a name="4"></a>
* AWS
  * CodePipeline: take inputs from many resources such as GitHub, AWS CodeCommit, AmazonECR, AmazoneS3
    * Stages call actions providers
      * AWS services
      * Third-party Actions
      * Custom Actions
      * Change configurations in *.yml
      * Build environment is a Docker container
  * CodeBuild: Build and test code with continuous scaling
* Azure:
  * Continuously Build, Test and Deploy to any platform and cloud
  * Open-source projects have unlimited build time and 10 parallel jobs for free
* Google Cloud Platform(GCP)
  * This is see the previous course about GCP. [DevOps - GCP](https://github.com/ph0123/Learning-Google-Cloud-Developer-and-DevOps-Tools)
## 5. Codes Repositories <a name="5"></a>
* GitHub 04_01 folder
* GitLab CI 04_02 folder
* Bitbucket Pipeline 04_03 folder




