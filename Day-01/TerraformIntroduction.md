# Terraform Introduction

Terraform is an open-source Infrastructure as Code (IaC) tool developed by HashiCorp. It allows you to define, provision, and manage infrastructure across various cloud providers using a declarative configuration language.

## Key Features

- **Platform Agnostic:** Supports multiple cloud providers (AWS, Azure, GCP, etc.).
- **Declarative Syntax:** Describe the desired state of your infrastructure.
- **Version Control:** Store configurations in source control for collaboration and auditing.
- **Resource Management:** Create, update, and delete infrastructure resources efficiently.

## Basic Workflow

1. **Write**: Define infrastructure in `.tf` files.
2. **Initialize**: Run `terraform init` to set up the working directory.
3. **Plan**: Use `terraform plan` to preview changes.
4. **Apply**: Execute `terraform apply` to provision resources.
5. **Destroy**: Remove resources with `terraform destroy` when no longer needed.

## Example

```hcl
provider "aws" {
    region = "us-west-2"
}

resource "aws_instance" "example" {
    ami           = "ami-0c55b159cbfafe1f0"
    instance_type = "t2.micro"
}
```

Terraform simplifies infrastructure management, making deployments more reliable and repeatable.