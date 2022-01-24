## Troubleshoot Terraform
In this tutorial, you will clone a repository with a broken Terraform configuration to deploy an EC2 instance and underlying networking. 

![Troubleshoot](https://user-images.githubusercontent.com/33342822/150720945-b343a351-ad14-4e99-bda2-3566e960f261.png)

### Format the configuration
The format command scans the current directory for configuration files and rewrites your Terraform configuration files .
- `terraform fmt`

### Validate your configuration
`terraform fmt` only parses your HCL for interpolation errors or malformed resource definitions, which is why you should use `terraform validate` after formatting your configuration to check your configuration in the context of the providers' expectations.
- `terraform validate`

### Reference
https://learn.hashicorp.com/tutorials/terraform/troubleshooting-workflow
