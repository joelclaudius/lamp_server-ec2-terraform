# Terraform EC2 Instance with LAMP Server Automation

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
- [Contributions](#contributions)
- [License](#license)

## Overview

Welcome to the Terraform project that deploys an EC2 instance and automates the installation of a LAMP (Linux, Apache, MySQL, PHP) server stack. This project streamlines the process of creating a web server in AWS and configuring it for web hosting.

## Project Structure

- **main.tf**: This file contains the Terraform code for creating the EC2 instance, specifying its attributes, and defining the security groups and key pair.

- **var.tf**: Here, you'll find the variables used in the creation of the EC2 instance, such as instance type, region, and your AWS access key and secret key.

- **output.tf**: This file provides the code to display the EC2 instance's public IP address and the SSH command needed to log in remotely.

- **install_lamp.sh**: The `install_lamp.sh` script is used as user data when launching the EC2 instance. It automates the installation and configuration of the LAMP server stack, making your web server ready for hosting web applications.

## Getting Started

To deploy your EC2 instance with the LAMP server stack, follow these steps:

1. Clone this repository to your local machine.

2. Open the `var.tf` file and update the variables to match your AWS credentials, preferred instance settings, and other configurations.

3. Run `terraform init` to initialize the project and download necessary providers.

4. Run `terraform apply` to create the EC2 instance and LAMP server stack.

5. The public IP address of your EC2 instance will be displayed upon successful completion of the deployment. You can use this IP address to access your web server.

6. You can also use the SSH command displayed to log in to your instance remotely.

## Contributions

Contributions are welcome! If you encounter any issues or have suggestions for improvement, please open an issue or create a pull request.
```bash 
git clone https://github.com/joelclaudius/lamp_server-ec2-terraform.git
```

## License

This project is free to use.


