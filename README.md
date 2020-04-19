# Basics
Create file main.tf

Add resources to it (e.g.)

```provider "aws" {
  region = "us-east-1"
}

resource "aws_instance" "example" {
  ami           = "ami-0c55b159cbfafe1f0"
  instance_type = "t2.micro"
}```

Run terraform commands
terraform init
# Good Tutorials

https://blog.gruntwork.io/an-introduction-to-terraform-f17df9c6d180#3ec6


https://learn.hashicorp.com/terraform/getting-started/intro