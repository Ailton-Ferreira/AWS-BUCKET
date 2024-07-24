# AWS-BUCKET

terraform {
    required_version = ">=1.3.0"
  required_providers {
    aws = {
      source = "hashicorp/aws"
      version = "5.59.0"
    }
  }
}

provider "aws" {

   region  = "us-west-2"
   default_tags {
     tags = {
       "owner" = "ailtongil" 
       managed-by ="terraform"
     }
   }
  
}
