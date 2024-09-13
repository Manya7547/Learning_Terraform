# 01 - Evolution of Cloud + Infrastructure as Code

In the early 90s and 2000s, tech companies building web applications had to go through a cumbersome process.

They needed to devise their idea, write the software, purchase servers, set up data centers, and handle all the power management, networking, and operational overhead. This process was challenging and time-consuming, often requiring significant capital expenses.

With the advent of cloud computing in the late 2000s and 2010s, the process changed drastically. After developing an idea and writing the software, companies could now deploy their applications to the cloud.

## Key Advantages of Cloud Infrastructure:

- Infrastructure available via APIs: Rather than needing to purchase and set up infrastructure, API driven systems can spin up or spin down servers as needed within minutes. This on-demand resource model made infrastructure management faster and more efficient.

- Speed and Flexibility: The ability to scale infrastructure up or down quickly in response to changing demands, like during high-traffic events such as Black Friday sales.

- Shift in Mindset: Infrastructure is now viewed as short-lived and immutable, as opposed to the long-lived and mutable model of traditional data centers. This means that when changes or updates are needed, new servers with the required dependencies are provisioned, and old ones are torn down.

The evolution of cloud infrastructure has revolutionized the way web applications are developed and deployed.

The shift from managing physical servers and data centers to leveraging on-demand resources through cloud providers has introduced speed, flexibility, and a new mindset around infrastructure management. This paradigm shift has led to the emergence of powerful tools like Terraform that make managing cloud infrastructure even more efficient and reliable.

## Infrastructure as Code Overview

Three Main Approaches for Provisioning Cloud Resources:

1. Cloud Console: A graphical user interface (GUI) provided by cloud providers, allowing users to interact with and manage cloud services.

2. API or Command-Line Interface: A method of interacting with cloud services programmatically, allowing for more efficient and automated management.

3. Infrastructure as Code: Defining your entire infrastructure within your codebase, offering better control, visibility, and consistency across environments.

### Categories of Infrastructure as Code Tools:

1. Ad-hoc scripts: Basic scripts that make API calls to provision infrastructure resources (e.g., shell scripts).

2. Configuration management tools: Tools like Ansible, Puppet, and Chef, designed to manage software and infrastructure configuration.

3. Server templating tools: Tools for building server templates, such as Amazon Machine Images (AMIs) or virtual machine images.

4. Orchestration tools: Tools like Kubernetes, which focus on deploying applications and managing containers.

5. Provisioning tools: Tools like Terraform, which focus on provisioning cloud resources using a declarative approach.

### Declarative vs. Imperative:

- Declarative tools define the desired end state of your infrastructure (e.g., five servers, one load balancer), and the tool handles the API calls and processes to achieve that state.
- Imperative tools require you to define the sequence of actions to create the desired infrastructure. What needs to happen and sequence of actions to take.

Terraform lies on the declarative side, we want to specify the end state that our infrastructure is going to take and you let the took handle how to actually get there.

## IaC Provisioning Tools Landscape

### Cloud-Specific vs. Cloud-Agnostic:

- Cloud-specific tools: These tools, such as AWS CloudFormation or Azure Resource Manager, are provided by major cloud providers and focus on provisioning infrastructure within their respective clouds. CloudFormation can't be used outside AWS.
- Cloud-agnostic tools: Tools like Terraform or Pulumi, which can be used across any cloud provider, allowing for greater flexibility when deploying resources across multiple clouds or when using third-party services.

Understanding Infrastructure as Code and the various approaches to provisioning cloud resources is essential for modern infrastructure management. By leveraging IaC tools, you can better control, maintain, and deploy your cloud infrastructure in a consistent, efficient, and scalable manner. As you plan your infrastructure, consider whether cloud-specific or cloud-agnostic tools would best suit your project's requirements and the potential need to span across multiple cloud providers.
