# Basics
Create file main.tf

Add resources to it (e.g.)

```

provider "aws" {
  region = "us-east-1"
}

resource "aws_instance" "example" {
  ami           = "ami-0c55b159cbfafe1f0"
  instance_type = "t2.micro"
}

```


Run terraform init - this tells Terraform to scan the code, figure out what providers you’re using, and download the code for them. Need to run init everytime you start on new terraform code

terraform init

Run terraform plan command

terraform plan


# Good Tutorials

https://blog.gruntwork.io/an-introduction-to-terraform-f17df9c6d180#3ec6


https://learn.hashicorp.com/terraform/getting-started/intro