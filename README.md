## Troubleshoot Terraform
In this tutorial, you will clone a repository with a broken Terraform configuration to deploy an EC2 instance and underlying networking. 

### Format the configuration
The format command scans the current directory for configuration files and rewrites your Terraform configuration files .
- `terraform fmt`

### Validate your configuration
`terraform fmt` only parses your HCL for interpolation errors or malformed resource definitions, which is why you should use `terraform validate` after formatting your configuration to check your configuration in the context of the providers' expectations.
- `terraform validate`

### Reference
https://learn.hashicorp.com/tutorials/terraform/troubleshooting-workflow