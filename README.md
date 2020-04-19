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

```terraform init```

Run terraform plan command. The plan command lets you see what Terraform will do before actually doing it. This is a great way to sanity check your changes before unleashing them onto the world.
Running plan is not required as you see the same output whilst running the appky command. However the plan command is good to run for a sanity check

```terraform plan```

Run terraform apply command.  This will show you the same plan output and asks you to confirm if you actually want to proceed with this plan. 

```terraform apply```

# Good Tutorials

https://blog.gruntwork.io/an-introduction-to-terraform-f17df9c6d180#3ec6

https://learn.hashicorp.com/terraform/getting-started/intro

https://blog.gruntwork.io/terraform-tips-tricks-loops-if-statements-and-gotchas-f739bbae55f9

https://blog.gruntwork.io/how-to-create-reusable-infrastructure-with-terraform-modules-25526d65f73d

https://learn.hashicorp.com/terraform/aws/lambda-api-gateway