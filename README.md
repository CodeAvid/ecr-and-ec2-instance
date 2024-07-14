# terraform-aws-ec2-ecr-manager

Welcome to the `terraform-aws-ec2-ecr-manager` repository! This project provides Terraform scripts to manage AWS EC2 and ECR instances efficiently. Use this guide to get started with setting up and managing your AWS infrastructure using Terraform.

## Table of Contents

1. [Introduction](#introduction)
2. [Prerequisites](#prerequisites)
3. [Installation](#installation)
4. [Configuration](#configuration)
5. [Usage](#usage)
6. [Examples](#examples)
7. [Contributing](#contributing)
8. [License](#license)

## Introduction

This repository contains Terraform scripts to help you manage AWS EC2 and ECR instances. Terraform is an Infrastructure as Code (IaC) tool that enables you to define and provision your infrastructure using code, making it easier to manage and scale your cloud resources.

## Prerequisites

Before you begin, ensure you have the following installed on your machine:

- [Terraform](https://www.terraform.io/downloads.html) (version 0.12 or higher)
- [AWS CLI](https://aws.amazon.com/cli/) (configured with your AWS credentials)
- An AWS account with the necessary permissions to manage EC2 and ECR resources

## Installation

1. Clone this repository to your local machine:
   ```sh
   git clone https://github.com/yourusername/terraform-aws-ec2-ecr-manager.git
   cd terraform-aws-ec2-ecr-manager


2. Initialize Terraform:
   ```sh
   terraform init
   ```

## Configuration

1. Copy the `terraform.tfvars.example` file to `terraform.tfvars`:
   ```sh
   cp terraform.tfvars.example terraform.tfvars
   ```

2. Edit the `terraform.tfvars` file to include your AWS configuration and desired settings:
   ```hcl
   aws_region       = "us-west-2"
   ec2_instance_type = "t2.micro"
   ecr_repository_name = "my-ecr-repo"
   ```

## Usage

1. Plan your Terraform deployment to see what changes will be made:
   ```sh
   terraform plan
   ```

2. Apply the Terraform scripts to create the resources:
   ```sh
   terraform apply
   ```

3. Destroy the Terraform-managed infrastructure when no longer needed:
   ```sh
   terraform destroy
   ```

## Examples

Here are some example configurations and their expected outcomes:

### Basic EC2 and ECR Setup

```hcl
aws_region       = "us-west-2"
ec2_instance_type = "t2.micro"
ecr_repository_name = "my-ecr-repo"
```

This configuration will create a `t2.micro` EC2 instance in the `us-west-2` region and an ECR repository named `my-ecr-repo`.

## Contributing

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository.
2. Create a new branch with a descriptive name.
3. Make your changes.
4. Submit a pull request with a detailed description of your changes.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to reach out if you have any questions or need further assistance. Happy Terraforming!
