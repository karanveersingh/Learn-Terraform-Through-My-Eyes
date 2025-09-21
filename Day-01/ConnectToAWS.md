# Connecting Terraform to AWS

To connect Terraform to AWS, follow these steps:

## 1. Install Terraform

Download and install Terraform from the [official website](https://www.terraform.io/downloads.html).

## 2. Configure AWS Credentials

Set up your AWS credentials using one of the following methods:

### a. AWS CLI

```sh
aws configure
```
Enter your AWS Access Key, Secret Key, region, and output format.

### b. Environment Variables

```sh
export AWS_ACCESS_KEY_ID="your-access-key-id"
export AWS_SECRET_ACCESS_KEY="your-secret-access-key"
export AWS_DEFAULT_REGION="your-region"
```

## 3. Create a Terraform Configuration

Create a file named `main.tf`:

```hcl
provider "aws" {
    region = "us-east-1"
}
```

## 4. Initialize Terraform

```sh
terraform init
```

## 5. Verify the Connection

Run:

```sh
terraform plan
```

If configured correctly, Terraform will connect to your AWS account.
