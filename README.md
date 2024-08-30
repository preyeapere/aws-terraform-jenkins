# aws-terraform-jenkins
This is a project that showcases the installation of jenkins and other AWS resources using Terraform (IAC)

# Error doing project
Error: Error launching source instance: Unsupported: The requested configuration is currently not supported. Please check the documentation for supported configurations.
│       status code: 400, request id: 5189cda7-abcd-4af8-aa0c-691e5330d728   
│
│   with aws_instance.jenkinsapp-server,
│   on jenkins-server.tf line 14, in resource "aws_instance" "jenkinsapp-server":
│   14: resource "aws_instance" "jenkinsapp-server" {

    #Solution
    I change my instance type file from t2. small to t3.micro