# 03 - Infrastructure as Code Overview

This section provides notes about

1. Overview of Terraform
2. How to set up Terraform and authorize it with AWS
3. Benefits of using Terraform and its compatibility with various cloud providers and services.

## Terraform Overview

Terraform is a powerful Infrastructure as Code (IaC) tool that allows you to build, change, and version infrastructure safely and easily.

## Benefits of Terraform:

- Apply software development best practices to infrastructure management.
- Utilize version control to track infrastructure changes over time.
- Cloud-agnostic approach allows for compatibility with multiple cloud providers and services.
- Interact with almost any online service with an API.

## Terraform with Other Tools:

Terraform can be used in conjunction with other IaC tools to create powerful and flexible infrastructure management solutions.

Some common patterns include:

1. Terraform + Configuration Management Tools (e.g., Ansible):
   Terraform provisions virtual machines
   Ansible installs and configures dependencies inside virtual machines.

2. Terraform + Templating Tools (e.g., Packer):
   Terraform provisions servers.
   Packer builds the image from which virtual machines are created.

3. Terraform + Orchestration Tools (e.g., Kubernetes):
   Terraform provisions Kubernetes clusters.
   Kubernetes defines how the application is deployed and managed on the cloud resources.

## Terraform Architecture:

![Alt text](/02-overview/terraform%20architecture.webp)

### Terraform consists of two main components:

1. Terraform Core:
   The engine that processes configuration files and manages the Terraform state file.
   Responsible for interacting with cloud provider APIs to make the current state match the desired configuration.

2. Terraform Providers:
   Plugins for Terraform Core that allow it to interact with specific cloud providers and services.
   Map configuration and state information to the appropriate API calls.
   Over 100 providers available for various cloud providers and services.
   In the next lesson, we will walk you through setting up Terraform on your system and configuring it to work with AWS.
