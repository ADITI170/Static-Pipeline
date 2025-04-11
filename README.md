# Static Website Deployment on AWS using Terraform

This project sets up a fully automated static website deployment pipeline using AWS services and Terraform Infrastructure as Code (IaC). It provisions:

- An S3 bucket configured for static website hosting.
- A CodeStar connection to GitHub (V2).
- An AWS CodePipeline that deploys changes automatically to the S3 bucket.

---

##Prerequisites

- [Terraform](https://developer.hashicorp.com/terraform/downloads)
- [AWS CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)
- An AWS account with admin-level access
- A GitHub repository with your static site files (HTML/CSS/JS)
- AWS credentials configured using `aws configure`

## Deployment Steps

### 1. Clone this Repository

```bash```
git clone https://github.com/YOUR-USERNAME/static-site-pipeline.git
cd static-site-pipeline


### 2. Configure AWS CLI (Provide your access key, secret key, region (e.g., us-east-1), and preferred output format.)
### 3. Create a CodeStar GitHub Connection
     -Connection is created via Terraform, you must approve it manually in the AWS Console.
### 3. Initialize and Deploy

# Teardown (To destroy all created AWS resources:)

cd main
terraform destroy
