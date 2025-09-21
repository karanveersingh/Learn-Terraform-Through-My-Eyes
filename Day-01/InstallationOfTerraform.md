# Installation of Terraform

Terraform is an open-source infrastructure as code (IaC) tool by HashiCorp. Follow these steps to install Terraform on your system.

## Prerequisites

- Supported operating system (Windows, macOS, or Linux)
- Internet connection

## Steps to Install Terraform

### 1. Download Terraform

- Visit the [Terraform Downloads Page](https://www.terraform.io/downloads.html).
- Select your operating system and architecture.
- Download the appropriate ZIP archive.

### 2. Install Terraform

#### On Windows

1. Extract the ZIP file.
2. Move the `terraform.exe` file to a directory included in your system's `PATH` (e.g., `C:\Windows\System32` or create a custom folder and add it to `PATH`).

#### On macOS/Linux

1. Extract the ZIP file:
    ```sh
    unzip terraform_<VERSION>_<OS>_amd64.zip
    ```
2. Move the binary to `/usr/local/bin`:
    ```sh
    sudo mv terraform /usr/local/bin/
    ```

### 3. Verify Installation

Open a terminal or command prompt and run:
```sh
terraform -version
```
You should see the installed Terraform version.

## Next Steps

- [Configure Terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)
- Start building your first infrastructure!
